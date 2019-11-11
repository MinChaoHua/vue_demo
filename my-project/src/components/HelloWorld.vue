<template>
  <div class="hello">
   <canvas id="myCanvas">

   </canvas>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  mounted: function() {
    this.creatCar();
  },
  methods: {
    creatCar() {
      var canvas = document.getElementById('myCanvas');
      var ctx = canvas.getContext('2d');
      ctx.beginPath();
      ctx.arc(100,75,50,0,2*Math.PI);
      ctx.stroke();
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
canvas { border: 1px solid black; }
</style>
