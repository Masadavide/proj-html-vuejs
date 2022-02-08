<template>
  <header>
      <Introduction />
      <Corses />
  </header>
</template>

<script>
import Introduction from './commons/Introduction.vue'
import Corses from './commons/Corses.vue'

export default {
  components: { 
    Introduction,
    Corses
  },
  name: 'Main',
  props: {
    msg: String
  }
}
</script>


<style scoped lang="scss">
  header{
    margin-top: 150px;
  }
</style>
