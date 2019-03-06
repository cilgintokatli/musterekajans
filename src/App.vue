<template>
  <div id="app">
    <div class="wrapper">
      <header>logo</header>
      <div class="slides">
        <div class="slide-1" :class="{active:selected == 1}">
          <img
            src="https://images.unsplash.com/photo-1518235506717-e1ed3306a89b?ixlib=rb-1.2.1&auto=format&fit=crop&w=1500&q=80"
            alt
          >
        </div>
        <div class="slide-2" :class="{active:selected == 2}">
          <img
            src="https://images.unsplash.com/photo-1502602898657-3e91760cbb34?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1504&q=80"
            alt
          >
        </div>
        <div class="slide-3" :class="{active:selected == 3}">
          <img
            src="https://images.unsplash.com/photo-1474606030380-107829a22fc6?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1500&q=80"
            alt
          >
        </div>
        <div class="slide-4" :class="{active:selected == 4}">
          <img
            src="https://images.unsplash.com/photo-1516710505574-0245114a1093?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1500&q=80"
            alt
          >
        </div>
        <div class="slide-5" :class="{active:selected == 5}">
          <img
            src="https://images.unsplash.com/photo-1494587416117-f102a2ac0a8d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1500&q=80"
            alt
          >
        </div>
      </div>
      <nav>
        <span @click="selected = 1" :class="{clicked:selected == 1}">new york</span>
        <span @click="selected = 2" :class="{clicked:selected == 2}">paris</span>
        <span @click="selected = 3" :class="{clicked:selected == 3}">london</span>
        <span @click="selected = 4" :class="{clicked:selected == 4}">istanbul</span>
        <span @click="selected = 5" :class="{clicked:selected == 5}">tokyo</span>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      selected: 1
    }
  }
};
</script>

<style lang="scss">
@import "../src/assets/scss/main.scss";
</style>
