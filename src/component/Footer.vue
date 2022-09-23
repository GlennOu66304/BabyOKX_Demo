<template>
  <div id="footer" class="section">
    <!-- text and logo -->
    <div>
      <img src="../assets/logo.jpg" alt="" />
      <span>BABYOKX 社区</span>
    </div>

    <!-- pasted board -->
    <div class="contract">
      <h2 class="contract-address" type="text">{{ message }}</h2>
      <img src="../assets/paste_03.jpg" alt="" />
      <h2
        v-clipboard:copy="message"
        v-clipboard:success="onCopy"
        v-clipboard:error="onError"
      >
        复制到粘贴板
      </h2>

      <!-- intro -->
      <!-- social media -->
      <!-- email -->
      <!-- copyright -->
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      message: "6666",
    };
  },
  mounted() {},
  methods: {
    onCopy: function () {
      alert("You just copied: " + this.message);
    },
    onError: function () {
      console.log();
      alert("Failed to copy texts");
    },
  },
};
</script>

<style>
#footer {
  height: 80vh;
  /* background-color: gold; */
}
.contract {
  display: flex;
}
img {
  height: 35px;
  margin-top: 15px;
  margin-left: 15px;
}
.contract-address {
  background-color: black;
  color: white;
}
</style>
