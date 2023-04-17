<template>
  <div>
    <the-header></the-header>
    <badge-list></badge-list>
    <user-info
      :full-name="activeUser.name"
      :info-text="activeUser.description"
      :role="activeUser.role"
    ></user-info>
  </div>
</template>

<script>
// local component registration
//Local registration scopes the availability of the registered components
//to the current component only. It makes the dependency relationship more explicit, and is more tree-shaking friendly.
import TheHeader from './components/TheHeader.vue';
import UserInfo from './components/UserInfo.vue';
import BadgeList from './components/BadgeList.vue';

export default {
  components: {
    'the-header': TheHeader,
    'user-info': UserInfo,
    'badge-list': BadgeList
  },
  data() {
    return {
      activeUser: {
        name: 'Maximilian Schwarzmüller',
        description: 'Site owner and admin',
        role: 'admin',
      },
    };
  },
};
</script>

<style>
html {
  font-family: sans-serif;
}

body {
  margin: 0;
}
</style>