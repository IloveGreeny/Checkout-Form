<script setup>
import {ref} from "vue";
import axios from "axios";

const apiImg = ref();

const fetchImg = () => {
  axios.get("https://dog.ceo/api/breed/bulldog/images/random")
      .then(response => {
        apiImg.value = response.data;
      })
      .catch(err => {
        console.log(err);
      })
}

fetchImg();


</script>

<template>
  <div style="background-color: gray ">
    <h1>Order Summary</h1>
    <main style="  border: 5px solid gray ; background-color: white;">
      <h2>Bulldog</h2>
      <ul>
        <li class="list" v-for="img in apiImg">
          <img :src="img" alt="dog" width="200" height="200"/>
        </li>
      </ul>
    </main>
  </div>
</template>



<style scoped>

</style>