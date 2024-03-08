<script setup>
import {RouterLink} from 'vue-router';
</script>


<template>
  <div>
    <header>
      <nav class="container">
        <div class="branding">
          <img src="../assets/Vue_Logo_Black.png" alt="">
          <h1>Vue Todos </h1>
        </div>
        <ul class="nav-routes">
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/about">About</RouterLink>

        </ul>
      </nav>
    </header>

  </div>
</template>



<style lang="scss" scoped>
header {
  background-color: #b1ecd7;
  nav {
    display: flex;
    align-items: center;
    padding: 25px 16px;

    .branding {
      display: flex;
      align-items: center;
      gap: 8px;
      img {
        max-width: 50px;
      }

      h1 {
        font-size: 24px;
        color: rgb(63, 60, 60);
      }
    }

    .nav-routes {
      display: flex;
      flex: 1;
      justify-content: flex-end;
      gap: 12px;
      color: rgb(63, 60, 60);
      list-style: none;

      a {
        text-decoration: none;
        color: inherit;
      }
    }
  }
}

</style>
