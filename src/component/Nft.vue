<template>
  <div class="nft">
    <h2>NFT</h2>

    <swiper
      :slides-per-view="3"
      :space-between="30"
      :loop="false"
      :pagination="true"
      :autoplay="true"
      :navigation="true"
      @swiper="onSwiper"
      @slideChange="onSlideChange"
    >
      <swiper-slide
        v-for="n in 5"
        :key="n"
        class="test"
        :class="{ test_2: true }"
      >
  
        <img
          :src="getImageUrl(34 + n)"
          width="600"
          height="400"
          class="img-fluid w-100 mx-auto"
          blank="true"
        />
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
// swiper-vue2
// https://github.com/Orest-2/swiper-vue2
// do not use the sass css, use the regular css
// Swiper Vue.js Components
// https://swiper6.vercel.app/vue#usage
import { Navigation, Pagination,Autoplay } from "swiper";

import { SwiperCore, Swiper, SwiperSlide } from "swiper-vue2";

// Import Swiper styles
import "swiper/swiper-bundle.css";

SwiperCore.use([Navigation, Pagination,Autoplay]);

export default {
  name: "Nft",

  components: {
    Swiper,
    SwiperSlide,
  },
  methods: {
    getImageUrl(imageId) {
      return `https://picsum.photos/600/400/?image=${imageId}`;
    },
    onSwiper(swiper) {
      console.log(swiper);
    },
    onSlideChange() {
      console.log("slide change");
    },
  },
};
</script>

<style scoped>
.img-fluid {
  max-width: 100%;
  height: auto;
}
.w-100 {
  width: 100%;
}
.ml-auto,
.mx-auto {
  margin-left: auto;
}
.mr-auto,
.mx-auto {
  margin-right: auto;
}
</style>
