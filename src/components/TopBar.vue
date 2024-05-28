<template>
  <header class="header">
    <nav>
      <RouterLink class="logo" to="/">
        <img height="40px" :src="logo"/>
      </RouterLink>
      <div class="link-list">
        <RouterLink class="link" to="/about">About</RouterLink>
        <RouterLink class="link" to="/about">Leaderboard</RouterLink>
        <RouterLink class="link" to="/about">Patch notes</RouterLink>
        <RouterLink class="link" to="/about">Blog</RouterLink>
        <RouterLink class="link" to="/about">Press</RouterLink>
        <RouterLink class="link" to="/about">Wiki</RouterLink>
        <RouterLink class="link" to="/about">
          <img :src="facebook"/>
        </RouterLink>
        <RouterLink class="link" to="/about">
          <img :src="twitter"/>
        </RouterLink>
      </div>
    </nav>
  </header>
</template>

<script>
import logo from "@/assets/images/logoHorizontal.png";
import facebook from "@/assets/images/facebook.png";
import twitter from "@/assets/images/twitter.png";
import {RouterLink} from "vue-router";

export default {
  name: 'TopBar',
  components: {RouterLink},
  data() {
    return {
      logo: logo,
      facebook: facebook,
      twitter: twitter
    }
  }
}
</script>

<style lang="scss" scoped>
.header {
  height: 60px;
  position: fixed;
  top: 0;
  right: 0;
  left: 0;
  background: rgba(16, 21, 36, 0.9);
  padding: 0 10px 0 20px;
  box-shadow: 0 0 16px rgba(0,0,0,0.9);
  z-index: 2000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000;

  nav {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .link-list {
      display: flex;
      align-items: center;

      .link {
        text-decoration: none;
        color: #DFFFFE;
        font-size: 1.8em;
        padding-right: 15px;
        display: flex;
      }
    }
  }
}
</style>