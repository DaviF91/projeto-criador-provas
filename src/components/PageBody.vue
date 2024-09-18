<template>
  <AddProva />
</template>



<script>
import AddProva from './AddProva.vue'

export default {
  name: 'PageBody',
  props: {
    msg: String
  },
  components: {
    AddProva
  }
}
</script>


<style scoped>

</style>
