<template>
  <div id="app">
    <div class="navbar-container">
      <div class="navbar-content">
        <router-link to="/">
          <i class="bx bxs-home bx-sm"></i>
        </router-link>
        <router-link to="/basket">
          <i class="bx bxs-basket bx-sm"></i>
        </router-link>
        <router-link to="/heart">
          <i class="bx bxs-heart bx-sm"></i>
        </router-link>
        <router-link to="/time">
          <i class="bx bxs-time-five bx-sm"></i>
        </router-link>
      </div>
    </div>
  </div>
  <router-view />
</template>

<style lang="less">
.navbar-container {
  width: 100%;
  position: fixed;
  bottom: 0;
  .navbar-content {
    padding: 20px;
    display: flex;
    justify-content: space-between;
    a {
      color: rgba(163, 163, 163);
      &.router-link-exact-active {
        color: rgba(255, 131, 62);
      }
    }
  }
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
* {
  font-family: "Josefin Sans", sans-serif;
  margin: 0px;
  padding: 0px;
}
</style>
