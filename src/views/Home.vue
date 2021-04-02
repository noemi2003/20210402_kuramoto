<template>
<div class="app">
  <div class="accordion" @click="show">
    <p>アコーディオン</p>
  </div>
  <div class="accordionBody" v-if="open">
    <p>アコーディオンの中身が入ります</p>
  </div>
</div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'Home',
  data(){
    return{
      open: false,
    }
  },
  methods:{
    show(){
      this.open = !this.open
    }
  }
}
</script>

<style scoped>
p{
  margin: 0;
  padding: 10px;
}
.app {
  border: 1px solid black;
  width: 30vw;
}
.accordion {
  background-color: rgb(218, 218, 218);
  height: 100%;
}

.accordionBody{

}
</style>