<template>
  <div id="app">
    <Header></Header>
    <main>
      <p>Ghbdtnl;l;</p>
    </main>
  </div>
</template>

<script>
import Header from './components/Header.vue';
export default {
  name: "app",
  components: {
    Header
  }
}
</script>

<style scoped>
div {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;

  main {
    margin-top: 120px;
    color: black;
  }
}
</style>
