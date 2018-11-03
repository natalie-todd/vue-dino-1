<template>
  <div id='app'>
<!-- Add in component, ex: <Todo /> -->
<Header />
  </div>
</template>

<script>
// import component from component path
import Header from './components/Header.vue';
import Joblist from './components/Joblist.vue';
export default {
  name: 'App',
  components: {
    Header,
    Joblist
    //test test
    
  }
};
</script>

<style lang='css'>
</style>
