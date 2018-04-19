<template>
  <svg width="500" height="300"></svg>
</template>


<script>
import datjs from './data.json'
const d3 = require('d3');

export default {

data(){
    return{
datjs: datjs
    }
},
  mounted: function(){

      var svg = d3.select(this.$el);

      

      function render(data){

        // Bind data
        var circles = svg.selectAll("circle").data(data);
        
        // Enter
        circles.enter().append("circle")
          .attr("r", 10)
.merge(circles)
          .attr("cx", function (d){ return d.x; })
          .attr("cy", function (d){ return d.y; });

        // Exit
        circles.exit().remove();
      }

      function type(d){
        d.x = +d.x;
        d.y = +d.y;
        return d;
      }

      
        render(datjs);
      
}

}
</script>



<style lang="scss" scoped>

circle{
  color: red;
  
}

</style>
