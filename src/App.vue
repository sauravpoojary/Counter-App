<!-- <script setup>
  import {ref} from "vue"
  let count = ref(0);

  const addToCount = () => {
    console.log("inc")
    count.value = count.value + 1;
  }

  const subToCount = () => {
    count.value = count.value - 1;
  }


</script> -->

<script>
  export default({
    
    data(){
      return {
        count : 0,
        name : "Saurav Poojary"
      }
    },
    methods : {
      addToCount(){
        this.count = this.count + 1
      },
      subToCount(){
        this.count = this.count - 1
      }

    }

  })
</script>

<template>
  <main>
    <div>
      <h1>Hey {{name}} Current count is</h1>
      <h2>{{count}}</h2>
      <button @click="addToCount()">+</button>
      <button @click="subToCount()">-</button>
    </div>
  </main>
</template>

<style scoped>
main{
  background-color: rgb(209, 219, 69);
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

div{
  text-align: center;
}

</style>
