<script setup>
import { RouterLink, RouterView } from 'vue-router';
import HomeView from "../src/views/HomeView/HomeView.vue";

</script>

<template>
  <header>
    <div class="wrapper">

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>

      <HomeView/>


    </div>
  </header>


</template>

<style scoped>

</style>
