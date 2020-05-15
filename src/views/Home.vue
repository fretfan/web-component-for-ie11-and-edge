<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <Comp1/>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';
import Comp1 from '@/components/Comp1.vue';

export default {
  name: 'Home',
  components: {
    HelloWorld,
    Comp1,
  },
};
</script>
