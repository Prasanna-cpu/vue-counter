


 <script setup>
    import {ref} from 'vue'  
    const count=ref(0)
    const addtoCount=()=>{
      console.log("Hello from add to count")
      count.value=count.value+1
    }

    const subtracttoCount=()=>{
      console.log("Hello from subtract to count")
      count.value=count.value-1
    }

    const resettoZero=()=>{
      console.log("Reset to zero")
      count.value=0
    }
</script>  


<!-- <script>
    export default{
      data(){
        return{
          count:0
        }
      },
      methods:{
        addtoCount(){
          this.count=this.count+1
        },

        subtracttoCount(){
          this.count=this.count-1
        },

        resettoZero(){
          this.count=0
        }

      }
    }
</script> -->

<template>
  <main>
    <div>
      <h3>Current count is ...</h3>
      <h2>{{ count }}</h2>
      <button @click="subtracttoCount">-</button>
      <button @click="addtoCount">+</button>
      <button @click="resettoZero">Reset</button>
    </div>
  </main>
</template>


<style scoped>
   main{
    background-color: orange;
    height: 20vw; 
    width : 30vw;
    justify-content: center;
    font-family: Arial, Helvetica, sans-serif;
    display: flex;
    align-items: center;
   }
</style>  










