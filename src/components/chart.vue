<template>
    <div id="tester">
    </div>
</template>

<script>
    let TESTER = document.getElementById('tester');
	Plotly.plot( TESTER, [{
	x: [1, 2, 3, 4, 5],
	y: [1, 2, 4, 8, 16] }], {
	margin: { t: 0 } } );
export default {
  name: 'chart',
  data () {
    return {
    }
  }
}
</script>
<style lang="scss">
    #tester {
        width:600px;
        height:250px;
    }
</style>