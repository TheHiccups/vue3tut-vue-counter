<script setup>
  import{ref} from "vue";

  const count = ref(0);
</script>


<template>
  <div class="container">
    <div class="counterapp">
    <h4>
      The current count is...
    </h4>
    <h1>{{ count }}</h1>
    <button @click="count--">-</button>
    <button @click="count++">+</button>
  </div>
  </div>
</template>

<style scoped>
  body, .container{
    margin:0;
    padding:0;
  }
  .container{
    background-color: aliceblue;
    width: 100vw;
    height: 100vh;

    display: flex;
    align-items: center;
    justify-content: center;
  }
  .counterapp{
    text-align: center;
  }
</style>