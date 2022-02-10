<template>
  <header class="fixed-top">
      <div class="ms_container">
        <Navbar />
        <div class="ms_bar">
          <div class="ms_icon text-center">
            <i class="fas fa-pencil-ruler"></i>
          </div>
          <div class="ms_icon text-center">
            <i class="far fa-circle"></i>
          </div>
          <div class="ms_icon text-center">
            <i class="fas fa-book"></i>
          </div>
          <div class="ms_icon text-center">
            <i class="fas fa-shopping-cart"></i>
          </div>
        </div>
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

  .ms_bar{
    position: absolute;
    right: -7px;
    top: 200px;
    padding: 10px;
    border-radius: 10px;
    border: 3px solid $color11;
    box-shadow: -1px 1px 5px 1px $color11;
    background-color: $color0;

    .ms_icon{
      cursor: pointer;
      &:hover{
        color: $color3;
      }
    }
  }




</style>
