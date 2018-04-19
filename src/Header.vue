<template>
  <header>
  
  
  <b-navbar toggleable="sm" type="dark" variant="info">
<b-navbar-brand href="#">
    <b-img v-bind:src='image' class="ml-4 mr-4" />
    Balloons
</b-navbar-brand>

  </b-navbar>









</header>
</template>

<script>
import image from './assets/black64.png'
export default {
  data(){
      return {
image: image
      }
  }
}
</script>


<style lang="scss" scoped>

</style>
