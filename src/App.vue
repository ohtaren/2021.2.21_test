<template>
  <div class="accordion">
    <h2 class="title" @click="toggle">アコーディオン</h2>
    <p class="description" v-show="show">アコーディオンの中身が入ります</p>
  </div>
</template>

<script>
export default {
  data(){
    return{
      show: false
    };
  },
  methods:{
  toggle: function(){
    this.show = !this.show;
   }
  }
};
</script>

<style>
.title{
  width: 50%;
  height: 50px;
  background-color: gainsboro;
  padding-top: 20px;
  padding-left: 10px;
  
}

</style>

