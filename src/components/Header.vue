<template>
    <section class="header">
        <header>
            <div class="header-container">
                <div id="nav">
                <router-link to="/">Home</router-link>
                <router-link to="/about">About</router-link>
                </div>
                <router-view/>
            </div>
        </header>
        <div class="header-fixed"></div>
    </section>
</template>

<script>
export default {

}
</script>

<style  scooped>
header {
  position: fixed;
  top: 0;
  width: 100vw;
  height: 115px;
  box-shadow: 0 2px 15px rgba(0, 0, 0, 0.12);
  display: flex;
  align-items: center;
  color: #fff;
  background: #333;
  z-index: 3;
}

.header-fixed {
    width: 100vw;
    height: 115px;
    z-index: 2;
    background: #333;
}

.header-container {
  width: 80vw;
  margin: 0 auto;
}

header .header-container #nav a {
  color: #fff;
}

header .header-container #nav a:hover::after  {
  background-color: #fff;
}

#nav {
  width: 20%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
}
</style>
