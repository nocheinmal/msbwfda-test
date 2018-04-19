<template>
    <b-container fluid class="my-3">

    <b-row>
<b-col offset="0" cols="12" offset-sm="2" sm="4" offset-md="2" md="4" offset-lg="1" lg="5" class="thumb first">{{balloons}}
  <br>
  <b-img v-bind:src='image' class="img_down "/> 
</b-col>
<b-col cols="12"  sm="4"  md="4"  lg="5" class="thumb second">{{signInUp[0]}}/{{signInUp[1]}}
  <br>
  <b-img v-bind:src='image' class="img_down "/>
</b-col>
    </b-row>
    
    <b-row>
<b-col offset="0" cols="12" offset-sm="2" sm="4" offset-md="2" md="4" offset-lg="1" lg="5" class="thumb third">{{analyze}}
  <br>
  <b-img v-bind:src='image' class="img_down "/>
</b-col>
<b-col cols="12"  sm="4"  md="4"  lg="5" class="thumb fourth">{{optimize}}
  <br>
  <b-img v-bind:src='image' class="img_down "/>
</b-col>
    </b-row>

    <b-row>
<b-col offset="0" cols="12" offset-sm="2" sm="4" offset-md="2" md="4" offset-lg="1" lg="5" class="thumb fifth">{{we}}
  <br>
  <b-img v-bind:src='image' class="img_down "/>
</b-col>
<b-col cols="12"  sm="4"  md="4"  lg="5" class="thumb sixth">{{contact}}
  <br>
  <b-img v-bind:src='image' class="img_down "/>
</b-col>
    </b-row>

  </b-container>

<!--
  <div class="container-fluid">
  <div class="row">
    <div class="col-offset-xs-0 col-xs-12 col-offset-sm-2 col-sm-4 col-offset-md-2 col-md=4 col-offset-lg-1 col-lg-5 thumb">{{balloons}}</div>
    <div class="col-offset-xs-0 col-xs-12 col-offset-sm-2 col-sm-4 col-offset-md-2 col-md=4 col-offset-lg-1 col-lg-5 ">{{signInUp[0]}}/{{signInUp[1]}}</div>
  </div>
  <div class="row">
    <div class="col-offset-xs-0 col-xs-12 col-offset-sm-2 col-sm-4 col-offset-md-2 col-md=4 col-offset-lg-1 col-lg-5 ">{{analyze}}</div>
    <div class="col-offset-xs-0 col-xs-12 col-offset-sm-2 col-sm-4 col-offset-md-2 col-md=4 col-offset-lg-1 col-lg-5 ">{{optimize}}</div>
  </div>
  <div class="row">
    <div class="col-offset-xs-0 col-xs-12 col-offset-sm-2 col-sm-4 col-offset-md-2 col-md=4 col-offset-lg-1 col-lg-5 ">{{we}}</div>
    <div class="col-offset-xs-0 col-xs-12 col-offset-sm-2 col-sm-4 col-offset-md-2 col-md=4 col-offset-lg-1 col-lg-5 ">{{contact}}</div>
  </div>
</div> -->
</template>


<script>
import image from './assets/down.png'
export default {
  data(){
      return{
           balloons:'What is Balloons',
      signInUp:['Sign in','Sign up'],
      analyze:'Analyze your Data',
      optimize:'Optimize your data',
      we:'Who are we',
      contact:'Contact',
      image:image
      }
  }
}
</script>


<style lang="scss" scoped>


$first: rgb(191, 211, 121);
$second: rgb(219, 138, 106);
$third: rgb(105, 162, 209);
$fourth: rgb(184, 134, 185);
$fifth: rgb(173, 113, 206);
$sixth: rgb(97, 126, 204);
.thumb{
  
 font-size: large;
 font-weight: 750;
  text-align: center;
  background-color: orange;
  border-style: solid;
  border-color: lightgrey;
  border-width: 0.5px;
  padding:  64px;


  }

  .first{
  background-color: $first;
}

.second{
  background-color: $second;
}
.third{
  background-color: $third;
}
 .fourth{
  background-color: $fourth;
}

.fifth{
  background-color: $fifth;
}
.sixth{
  background-color: $sixth;
}


  


</style>
