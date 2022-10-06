<template>

  <div id="app">
    <Header />
 
     <b-container class="bv-example-row" fluid>
      <b-row>
        <!-- home -->
        <Home />
        </b-row> 

        <b-row>
        <!-- 关于我们 -->
        <About />
      </b-row>
      <!-- NFT -->

      <b-row>
        <Nft />
      </b-row>
      <b-row>
        <!-- 路线图 -->
        <RoadMap class="road-map"/>
      </b-row>
      <b-row class="FAQ">
        <!-- 常见问题 -->
        <FAQ />
      </b-row>
      <b-row>
        <!-- footer -->
        <Footer class="footer"/>
      </b-row>
   </b-container>
  </div>
   
</template>

<script>
import Header from "./component/Header.vue";
import Home from "./component/Home.vue";
import About from "./component/About.vue";
import Nft from "./component/Nft.vue";
import RoadMap from "./component/Roadmap.vue";
import FAQ from "./component/FAQ.vue";
import Footer from "./component/Footer.vue";
export default {
  name: "App",
  components: { Header, Home, About, Nft, RoadMap, FAQ, Footer },
};
</script>

<style>
body {
  font-family: sans-serif;
  background-color: black;
  color: white;
  scrollbar-width:none
  /* overflow:-Scroll;
  overflow-y:hidden */
}

/* margin-top: 30px; */

/* section */
.section {
  height: 1012px;
}
.aboutus{
  background-image: url(./assets/home-bg.png);
  color:white;
}
.road-map{
  background-color: #1b1d56;
}
.FAQ{
  background-color:#1b1d56;
}
.footer{
  background-image: url(./assets/footer_02.jpg);
}
</style>
