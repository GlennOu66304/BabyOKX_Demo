<template>
  <div id="app">
    <Header/>
    <!-- home -->
    <Home />
    <!-- 关于我们 -->
    <About />
    <!-- NFT -->
    <Nft />
    <!-- 路线图 -->
    <RoadMap />
    <!-- 常见问题 -->
    <FAQ />
    <!-- footer -->
    <Footer />
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
  components: { Header,Home, About, Nft, RoadMap, FAQ, Footer },
};
</script>

<style>
body {
  font-family: sans-serif;
  background-color: black;
  color: white;
}

/* margin-top: 30px; */

/* section */
.section {
   /* height: 80vh; */
}
</style>
