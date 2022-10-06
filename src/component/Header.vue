<template>
  <!-- nav bar -->
    <nav class="header" style="position:absolute; z-index:2;">
      <!-- logo -->
      <div class="logo" v-scroll-to="'#home'">
        <img src="../assets/logo.jpg" alt="" />
        <span>BABYOKX</span>
      </div>
      <ul class="links">
        <li v-scroll-to="'#about-us'">
          <h6>关于我们</h6>
        </li>
          <li v-scroll-to="'#nft'">
          <h6>NFT</h6>
        </li>
        <li v-scroll-to="'#roadmap'">
          <h6>路线图</h6>
        </li>
        <li v-scroll-to="'#faq'">
          <h6>常见问题</h6>
        </li>
      </ul>
      <div class="language">简体中文</div>
    </nav>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style>

.header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  color: white;
}
nav {
  display: flex;
}
.logo {
  margin-top: auto;
  align-items: center;
}
.links {
  display: flex;
  list-style-type: none;
  margin: auto;
}

li {
  margin-right: 20px;
}
.language{
  margin-top:20px;
}
</style>
