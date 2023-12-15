<template>
  <section>
    <h1>ชื่อ-นามสกุล : {{getFullName()}}</h1>
    <h1>{{age}}</h1>
    <p><span v-html="address"></span></p>
    </section>
</template>

<script>
export default {
  name: 'App',
  data(){
    return{
      firstName:"Nipapatr",
      lastName: "Kammun",
      age:20,
      address:"<strong>กทม</strong>"
    }
  },
  methods:{
    getFullName(){
      return this.firstName +" "+ this.lastName
    }
  }
}
</script>

<style>

</style>
