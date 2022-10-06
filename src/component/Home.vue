<template>
  <div id="home" class="section">
    <div class="left" style="position:relative; z-index:auto;">
    <h2>BabyOKX是OKX生态第一模因</h2>
    <div class="buttons">
      <b-button variant="primary" class="button">前往购买</b-button>
      <b-button variant="primary" class="button">查看图表</b-button>
    </div>

    <!-- 深入理解CSS中的层叠上下文和层叠顺序
    https://www.zhangxinxu.com/wordpress/2016/01/understand-css-stacking-context-order-z-index/ -->

    <div class="feature" style="position:absolute; z-index:2;">
      <Feature />
         <Feature />
            <Feature />
               <Feature />
              <Feature />
                     <Feature />
    </div>
    
</div>
<div class="right" style="position:relative; z-index:auto;">
 <img class="dog" src="../assets/dog_03.jpg" alt="" style="position:relative; z-index:1;"/>
</div>
   
  </div>
</template>

<script>
import Feature from "./Feature.vue";
export default {
  name: "Home",
  components: {
    Feature,
  },
};
</script>

<style>
#home {
  background-size: cover;
  background-position: center;
  background-image: url(../assets/home-bg.png);
  color: white;
  display: flex;

}
.left {
 margin-top:300px; 
  padding-left:150px;

}
.buttons {
  display: flex;
  margin-top:72px;
}
.button{
  margin-right: 35px;
}
.feature{
  margin-top:170px;
  display: flex;
}
.right{
  /* position: absolute; */


}
.dog {
  width: 574px;
  height: 647px;

}
</style>
