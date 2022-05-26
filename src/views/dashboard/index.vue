<template>
  <div>
    <Card></Card>
    <Sale></Sale>
    <Observe></Observe>
  </div>
</template>

<script>
import Sale from './Sale'
import Card from './Card'
import Observe from './Observe'
export default {
  name: '',
  components:{
    Card,
    Sale,
    Observe
  },
  mounted(){
    this.$store.dispatch('getData');
    console.log('--进入home--')
  }
}
</script>

<style scoped>

</style>
