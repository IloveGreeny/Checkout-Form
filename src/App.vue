<script setup>
import { RouterLink, RouterView } from 'vue-router'
import CheckoutForm from "../src/components/CheckoutForm/CheckoutForm.vue";

</script>

<template>
  <header>
    <div class="wrapper">

      <CheckoutForm/>



      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>

</style>
