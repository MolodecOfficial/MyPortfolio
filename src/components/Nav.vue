<script setup lang="ts">

</script>

<template>
  <section class="nav">
    <div class="nav_logo">
      <code>Molodec_Official 😺</code>
    </div>
    <section class="nav_menu">
      <a href="">Home</a>
      <a href="">About</a>
      <a href="">Projects</a>
      <a href="">Contact me</a>
    </section>
  </section>
</template>

<style scoped>
.nav {
  margin-top: 30px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.nav_logo {
  cursor: default;
  margin-left: 40px;
  color: white;
  font-size: clamp(7px, 2.5vw, 25px);
  transition: all 0.1s ease-in-out;
  &:hover {
    color: wheat;
  }
}
.nav_menu {
  gap: clamp(20px, 2.5vw, 45px);
  margin-right: 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  &.nav_menu a {
    font-family: Poppins, sans-serif;
    color: white;
    text-decoration: none;
    font-size: clamp(8px, 1.5vw, 25px);
    transition: all 0.2s ease-in-out;
    &:hover {
      color: wheat;
    }
  }
}

</style>