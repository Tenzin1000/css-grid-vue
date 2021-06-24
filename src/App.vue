<template>
<div id="main">
  <app-body></app-body>
</div>
</template>

<script>
import body from './comp/body.vue'
export default {
  components:{
    'app-body':body
  },
  data () {
    return {

    }
  }
}
</script>

<style>
  #main{
   max-width:1480px;
   margin: 40px 20px;
  }
</style>
