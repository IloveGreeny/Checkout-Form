<script setup>

const payment = () => {
  console.log("Payment Confirmed")
}

</script>


<template>

  <div class="bg">
    <h1>Payment Information</h1>
    <main class="border">
      <img src="../../assets/credit.png" alt="card"/>
      <div>
        <p> Name on Card</p>
        <input type="text"/>
        <p>Card Number</p>
        <input type="text"/>
        <p>Expiration Date</p>
        <input type="text" placeholder="Month"/>
        <input type="text" placeholder="Year"/>
        <p>
          CVC
        </p>
        <input type="text"/>
      </div>
      <button @click="payment()">Confirm Payment</button>
    </main>
  </div>


</template>



<style scoped>
.bg {
  background-color: gray;
}

.border {
  border: 5px solid gray ;
  background-color: white;
}
</style>