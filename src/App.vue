<template>
<div>
<app-header></app-header>
<app-main></app-main>
<app-footer></app-footer>
</div>
</template>

<script>

import Main from './Main.vue'
import Header from './Header.vue'
import Footer from './Footer.vue'

export default {
 
  data () {
    return {
     
    }
  },
  
  
  components:{
'app-main':Main,
'app-header':Header,
'app-footer':Footer
      
  }
}
</script>

<style lang="scss" scoped>
div{
background-color:#ccccb3;
}
</style>
