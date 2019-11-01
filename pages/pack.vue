<template>
    <div class="con">
        <h1>Hello  {{name}}</h1>
        <input type="text" v-model="name"> <br><br>
        <h2>enter change   {{name}}</h2>
        <input type="text" v-model="Nname" v-on:keyup.enter="changename">
        <button @click="changename">Click to change</button>
    </div>
    
</template>

<script>
export default {
    data(){
       
        return{
            name:'STPACK',
            Nname:''

        }
    },
    methods:{
        changename(){
            this.name=this.Nname,
            this.Nname=''

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