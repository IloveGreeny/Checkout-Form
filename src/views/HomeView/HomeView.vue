<script setup>
import {RouterView} from "vue-router";
import FetchData from "../../components/FetchData/FetchData.vue";
</script>






<template>
  <div>
      <h1>
        Welcome  to Dog app
      </h1>
    <FetchData/>
  </div>
  <RouterView/>
</template>


<style scoped>



</style>