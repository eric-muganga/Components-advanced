<template>
  <header>
    <h1>More on Vue Components</h1>
  </header>
</template>

//When a style tag has the scoped attribute, its CSS will apply to elements of the current component only.
<style scoped>
  header {
    width: 100%;
    height: 5rem;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #14005e;
  }

  header h1 {
    color: white;
    margin: 0;
  }
</style>