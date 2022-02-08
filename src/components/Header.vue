<template>
  <header class="fixed-top">
      <div class="ms_container">
        <Navbar />
      </div>
  </header>
</template>

<script>
import Navbar from './commons/Navbar.vue'


export default {
  components: { 
    Navbar,
  },
  name: 'Header',
  props: {
    msg: String
  }
}
</script>


<style scoped lang="scss">
@import '../assets/style/variables.scss';

  header{
    box-shadow: 0px 3px 2px $color11;
    background-color: $color0;
  } 




</style>
