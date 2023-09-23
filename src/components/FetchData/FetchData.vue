<script setup>

import {ref} from "vue";
import axios from "axios";

const apiData = ref(null);
const apiImg = ref();
const count = ref(0);

const fetchData = () => {
  axios.get("https://dog.ceo/api/breeds/list/all")
      .then(response=>{
        apiData.value = response.data;
      })
      .catch(err => {
        console.error(err);
      })

}

const fetchImg = () => {
  axios.get("https://dog.ceo/api/breed/bulldog/images/random")
      .then(response => {
        apiImg.value = response.data;
      })
      .catch(err => {
        console.log(err);
      })
}



</script>

<template>

  <div>
    <button @click="fetchData();fetchImg();count++">Fetch Data</button>
    <div v-if="apiData">
      <ul>
        <li class="list" v-for="item in apiData">
          <p>  {{item.bulldog}}</p>
        </li>
        <li class="list" v-for="img in apiImg">
          <img :src="img" alt="dog"/>
        </li>
      </ul>
    </div>
  </div>

</template>



<style scoped>

.list {
  list-style-type: none;
}

</style>