<template>
  <div id="app">
    <h1>Peace</h1>
    <message>Peace be Upon you !!</message>
    <chart></chart>
  </div>
</template>

<script>
import Message from './components/message.vue'
import Chart from './components/chart.vue'
export default {
  name: 'app',
  components: {Message, Chart},
  data () {
    return {
    }
  }
}
</script>

<style lang="scss">

</style>
