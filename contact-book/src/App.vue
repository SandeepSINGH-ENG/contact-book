<script setup>
</script>

<template>
  <div class="main-box">
    <nav>
      <ul>
       <li><img src="/vite.svg"</li>
        <li><router-link to="/">CONTACT BOOK <img src="./assets/book.svg"></router-link></li>
        <li><router-link to="/add">ADD NEW<img src="./assets/add.svg"></router-link></li>
      </ul>
    </nav>
    <router-view></router-view>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
