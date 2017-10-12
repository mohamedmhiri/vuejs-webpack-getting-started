<template>
  <div id="app">
    <h1>Peace</h1>
    <message>Peace be Upon you !!</message>
    <chart :chart-data="datacollection"></chart>
  </div>
</template>

<script>
import Message from './components/message.vue'
import Chart from './components/.vue'
export default {
  name: 'app',
  components: {Message, },
  data () {
    return {
      datacollection: [],
      date: []
    }
  },
  created () {
    this.date = this.datacollection.datasets.map(a => a.date)
    this.datacollection = {
      labels: this.date,
      datasets: [
        {
          label: 'Expense',
          backgroundColor: '#f87979',
          data: [
            {
                date: "April 15th 2017",
                expense: 100,
                income: 4000
            },
            {
                date: "April 22nd 2017",
                expense: 500,
                income: 2000
            },
            {
                date: "April 24th 2017",
                expense: 1000,
                income: 2300
            },
            {
                date: "April 29th 2017",
                expense: 2000,
                income: 1234
            },
            {
                date: "May 1st 2017",
                expense: 500,
                income: 4180
            },
            {
                date: "May 5th 2017",
                expense: 4000,
                income: 5000
            },
        ]
        },
        {
          label: 'Income',
          backgroundColor: '#5bf8bf',
          data: [
            {
                date: "April 15th 2017",
                expense: 100,
                income: 4000
            },
            {
                date: "April 22nd 2017",
                expense: 500,
                income: 2000
            },
            {
                date: "April 24th 2017",
                expense: 1000,
                income: 2300
            },
            {
                date: "April 29th 2017",
                expense: 2000,
                income: 1234
            },
            {
                date: "May 1st 2017",
                expense: 500,
                income: 4180
            },
            {
                date: "May 5th 2017",
                expense: 4000,
                income: 5000
            },
        ]
        }
      ]
    }
 },
 mounted () {
    this.date = this.datacollection.datasets.map(a => a.date)
    this.datacollection = {
      labels: this.date,
      datasets: [
        {
          label: 'Expense',
          backgroundColor: '#f87979',
          data: [
            {
                date: "April 15th 2017",
                expense: 100,
                income: 4000
            },
            {
                date: "April 22nd 2017",
                expense: 500,
                income: 2000
            },
            {
                date: "April 24th 2017",
                expense: 1000,
                income: 2300
            },
            {
                date: "April 29th 2017",
                expense: 2000,
                income: 1234
            },
            {
                date: "May 1st 2017",
                expense: 500,
                income: 4180
            },
            {
                date: "May 5th 2017",
                expense: 4000,
                income: 5000
            },
        ]
        },
        {
          label: 'Income',
          backgroundColor: '#5bf8bf',
          data: [
            {
                date: "April 15th 2017",
                expense: 100,
                income: 4000
            },
            {
                date: "April 22nd 2017",
                expense: 500,
                income: 2000
            },
            {
                date: "April 24th 2017",
                expense: 1000,
                income: 2300
            },
            {
                date: "April 29th 2017",
                expense: 2000,
                income: 1234
            },
            {
                date: "May 1st 2017",
                expense: 500,
                income: 4180
            },
            {
                date: "May 5th 2017",
                expense: 4000,
                income: 5000
            },
        ]
        }
      ]
    }
 }
}
</script>

<style lang="scss">

</style>
