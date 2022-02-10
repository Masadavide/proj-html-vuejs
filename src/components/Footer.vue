<template>
  <footer>
    <Newsletter />
    <Footer />
  </footer>
</template>

<script>
import Newsletter from './commons/Newsletter.vue'
import Footer from './commons/Footer.vue'


export default {
  components: { 
    Newsletter,
    Footer
  },
  name: 'Header',
  props: {
    msg: String
  }
}
</script>


<style scoped lang="scss">
@import '../assets/style/variables.scss';






</style>
