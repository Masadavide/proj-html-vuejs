<template>
  <main>
      <Introduction />
      <Corses />
      <Benefits />
      <Companionship />
      <Reviews />
      <Certification />
      <Blog />
  </main>
</template>

<script>
import Introduction from './commons/Introduction.vue'
import Corses from './commons/Corses.vue'
import Benefits from './commons/Benefits.vue'
import Companionship from './commons/Companionship.vue'
import Reviews from './commons/Reviews.vue'
import Certification from './commons/Certification.vue'
import Blog from './commons/Blog.vue'

export default {
  components: { 
    Introduction,
    Corses,
    Benefits,
    Companionship,
    Reviews,
    Certification,
    Blog
  },
  name: 'Main',
  props: {
    msg: String
  }
}
</script>


<style scoped lang="scss">
  main{
    margin-top: 150px;
    overflow-x: hidden;
  }
</style>
