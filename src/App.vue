<template>
  <div class="navbar-container">
    <div class="navbar-content">
      
      <router-link to="/">
        <i class='bx bx-home bx-sm'></i>
      </router-link>

      <router-link to="/basket">
        <i class='bx bx-basket bx-sm'></i>
      </router-link>

      <router-link to="/favorites">
        <i class='bx bx-heart bx-sm'></i>
      </router-link>

      <router-link to="/history">
        <i class='bx bx-history bx-sm' ></i>
      </router-link>

    </div>
  </div>
  <router-view/>
</template>

<style lang="less">

@import url('https://fonts.googleapis.com/css2?family=Josefin+Sans:wght@300&display=swap');

.navbar-container{
  width: 100%;
  position: fixed;
  bottom: 0;
  background: #fff;
  border-top: 1px solid #eee;
  .navbar-content{
    padding: 20px;
    display: flex;
    justify-content: space-between;
      a{
        color: rgba(163, 163, 163);
        &.router-link-exact-active {
        color: rgba(255, 131, 62);
      }
    }
  }
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

*{
  font-family: 'Josefin Sans', sans-serif;
  margin: 0;
  padding: 0;
}

::-webkit-scrollbar {
  width: 0;
  height: 0;
}

</style>
