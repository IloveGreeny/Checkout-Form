<script setup>
import { RouterLink, RouterView } from 'vue-router';
import HomeView from "../src/views/HomeView/HomeView.vue";

</script>

<template>
  <header>
    <div class="wrapper">

      <nav>

        <RouterLink class="text"  to="/">Home</RouterLink>

        <RouterLink class="text" to="/cart"> Shop Cart</RouterLink>
      </nav>

      <HomeView/>


    </div>
  </header>


</template>

<style scoped>

.text {
  text-decoration: none;
}

</style>
