<template>
  <div id='app'>
<!-- Add in component, ex: <Todo /> -->
<Joblist />
  </div>
</template>

<script>
// import component from component path
import Joblist from "./components/Joblist.vue";
export default {
  name: "App",
  components: {
    Joblist
  }
};
</script>

<style>
</style>
