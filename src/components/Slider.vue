<template>
  <div class="slider">
      <button type="button" class="btn btn-left">
          <img src="./../assets/chevron-left.svg" class="icone">
      </button>
      <div class="container-slides" :style="{transform: `translatex(${index}px)`,transition:`${transition}`}">
          <img src="./../assets/slider1.jpg"  class="img-slider">
           <img src="./../assets/slider2.jpg"  class="img-slider">
            <img src="./../assets/slider3.jpg"  class="img-slider">
             <img src="./../assets/slider4.jpg"  class="img-slider">
              <img src="./../assets/slider5.jpg"  class="img-slider">
      </div>
        <button @click="next" type="button" class="btn btn-right">
          <img src="./../assets/chevron-right.svg" class="icone">
      </button>
  </div>
</template>

<script>
export default {
      name:'Slider',
      data: function(){
          return{
              index: 0,
              transition:"transform 0.7s ease"
          }
      },
      methods:{
          next(){
              //console.log(this.index)
              if (this.index===-2000){
                  this.transition ="none";
                  this.index = 0;
              }else{
                  this.transition ="transform 0.7s ease"
                  this.index -=500;
              }
          }
      }
}
</script>

<style scoped>
  .slider{
      width: 100%;
      height: 300px;
      margin: 50px auto 0;
      overflow: hidden;
      position: relative;
  }
  .container-slides{
      display: flex;
  }
  .img-slider{
      width: 100%;
      height: 300px;
  }
  .btn{
      outline: none;
      border: none;
      width: 50px;
      height: 50px;
      border-radius: 50%;
      display: block;
      position:absolute;
      z-index: 1000;
      cursor: pointer;
      display: flex;
      justify-content: center;
      align-items: center;
  }
  .icone{
      width: 120px;

  }
  .btn-left{

      top:50%;
      left: 5px;
      transform: translateY(-50%);
  }
    .btn-right{
      top:50%;
      right: 5px;
      transform: translateY(-50%);
  }
</style>