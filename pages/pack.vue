<template>
    <div class="con">
        <h1>Hello  {{name}}</h1>
        <input type="text" v-model="name">
    </div>
    
</template>

<script>
export default {
    data(){
        return{
            name:'STPACK',
        }
    }
}
</script>

<style>
  .con {
     text-align: center;
     margin-top: 1rem;
  }
  </style>