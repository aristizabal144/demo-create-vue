<template>
  <div class="home">
    <Button label="Danger" class="p-button-danger" @click="console()"/>
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>

    <h1 class="title">Hola mundo</h1>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src
import Button from 'primevue/button';


export default Vue.extend({
  name: 'Home',
  components: {
    HelloWorld,
    Button
  },
  methods:{
    console(){
      console.log("oprimi el boton");
    }
  }
});
</script>

<style lang="scss" scoped>
.title{
  color: $color-primary-company;
}
</style>
