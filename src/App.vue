<template>
 <div id="app">
    <HelloWorld msg="You like avenger to tanos?" />
    <br>
    <div class="row">
      <div class="col-12">
      <img src="https://f.ptcdn.info/839/046/000/ofnpom5xdUDwFdo3Nei-o.jpg" width="200" height="300" />
        <h1>{{total1}}</h1>
        <div class="col-12">
          <CsButton @cc="sum" /><br>
        </div>
      </div>
      <div class="col-12">
      <img src="https://i.pinimg.com/474x/6f/76/39/6f7639e90ffb39a08759dcc160a843d7.jpg" width="200" height="300" />
        <h1>{{total2}}</h1>
        <div class="col-12">
          <CsButton @cc="sum1" />
        </div>
      </div>
    </div>
    
  </div>
</template>
<script>
import HelloWorld from "./components/HelloWorld.vue";
import CsButton from "./components/CsButton";
export default {
  name: "App",
  components: {
    HelloWorld,
    CsButton,
    
  },
  data : function(){
    return {
    total1: 0,
    total2: 0,
   
   } 
  },
  methods: {
  sum(counterValue){
    this.total1 = counterValue
  },
  
  sum1(counterValue){
    this.total2 = counterValue
},
},

};

</script>

<style>
body {
      background-image: url(https://a-static.besthdwallpaper.com/ewnecch-rs-infinity-sngkhraamolokbnphuuenhlangkrancch-wx-ll-pepexr-2560x1600-1756_7.jpg);
      background-size: auto ;
    }
#app {
  font-family: 'Londrina Solid', cursive;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  margin-top: 70px;
}
</style>