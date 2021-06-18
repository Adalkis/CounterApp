<template>
  <q-page class="flex flex-center" style="justify-content: space-evenly; background:#CFE8E7">
    <q-btn round icon="remove"  @click="decrease" class="buttons"/>
    <div style="width:200px; height:200px; background: #9ED0C9; border-radius:10px">
      <h1 style=" color:#415164; text-align:center ">{{counter}}</h1>
    </div>
    
    <q-btn round icon="add" @click="increase" class="buttons"/>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
  data(){
    return{
      counter:0
    }
  },
  methods:{
    increase(){
     this.counter++
     console.log(this.counter)
    },
    decrease(){
      this.counter--
     console.log(this.counter)

    }
  }
}
</script>

<style scoped>
.buttons{
  width:100px;
  height: 100px;
  background: #415164;
  color: #9ED0C9;
  font-size: 30px;
  
}
</style>
