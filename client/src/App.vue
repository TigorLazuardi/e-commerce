<template>
  <div id="app">
    <router-view />
  </div>
</template>

<script>
export default {};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  max-width: 100vw;
}

#app {
  display: flex;
  flex-direction: column;
}
</style>
