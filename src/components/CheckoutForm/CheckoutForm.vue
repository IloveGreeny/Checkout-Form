<script setup>

</script>

<template>
  <div>
    <h1>Payment Information</h1>
  </div>
  <div>
    <main>
      <img src="../../assets/credit.png" alt="card" width="318" height="207"/>
      <div>
        <h1>
          Name on card
        </h1>
        <input type="text"/>
        <div>
          <h1>
            Card Number
          </h1>
          <input type="text"/>
        </div>
        <div>
          <h1>
            Expiration date
          </h1>
          <input type="text" placeholder="Month"/>
          <input type="text" placeholder="Year"/>
          <h1>
            CVC
          </h1>
          <input type="text"/>
        </div>
      </div>
      <br>
      <div>
        <button>Confirm Payment</button>
      </div>

    </main>
  </div>

</template>



<style scoped>

</style>