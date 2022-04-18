<template>
  <nav class="navigation-bar">
    <div class="test">
      <i class="fa-solid fa-ghost"></i>
      <router-link to="/">Non Urgent Dilvery System</router-link>
    </div>
    <Login @toogleLoginTab="toogleLogin"/>
    <div class="test2">
      <router-link to="/about">About</router-link> 
      <router-link class="test3" to="/about">About</router-link> 
      <router-link class="test3" to="/about">About</router-link>
    </div>
  </nav>
    <LoginForm :toggleIfPressed="toogleIfPressed"/>
  <router-view class="z-0"/>
</template>
<script>
  import Login from "./components/Login.vue"
  import LoginForm from "./components/LoginForm.vue"
  export default {
    name: "App",
    components: {
      Login,
      LoginForm,
    },
    data() {
      return {
        toogleIfPressed: false,
      }
    },
    methods: {
      toogleLogin() {
        this.toogleIfPressed = !this.toogleIfPressed 
      }
    }
  }
</script>
<style>
  .navigation-bar {
    @apply  bg-primary text-white flex flex-nowrap border-b-[1px] border-gray-700 shadow-md shadow-primary font-Lobster;
    }
  .navigation-bar .test {
    @apply ml-2 text-lg p-2 w-1/2;
  }
  .navigation-bar .test i {
    @apply mr-2 text-[15px];
  }
  .navigation-bar .test a {
    @apply tracking-tighter
  }
  .navigation-bar .test2 {
    @apply w-1/2 flex justify-end mr-6  py-3 text-sm;
  }
  .navigation-bar .test2 a {
    @apply ml-3 ;
  }
  .navigation-bar .test3 {
    @apply border-l-2 pl-3
  }
  
</style>
