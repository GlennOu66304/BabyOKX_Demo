<template>
  <!-- nav bar -->
    <nav class="header">
      <!-- logo -->
      <div class="logo" v-scroll-to="'#home'">
        <img src="../assets/logo.jpg" alt="" />
        <span>BABYOKX</span>
      </div>
      <ul class="links">
        <li v-scroll-to="'#about-us'">
          <h1>关于我们</h1>
        </li>
        <li v-scroll-to="'#roadmap'">
          <h1>路线图</h1>
        </li>
        <li v-scroll-to="'#faq'">
          <h1>常见问题</h1>
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
