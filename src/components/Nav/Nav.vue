<template>
  <nav class="nav">
    <span class="nav__anime"></span>
    <div class="container">
      <div class="nav__box">
        <routerLink to="/" class="nav__logo">
          <h1>Omina Muhammad</h1>
        </routerLink>
        <button class="nav__burger" @click="burger = true">
          <img src="../../assets/images/burger.svg" alt="" />
        </button>
        <ul class="nav__list" :class="{ active: burger }">
          <button class="nav__close" @click="burger = false">
            <img src="../../assets/images/close.svg" alt="" />
          </button>
          <li>
            <button  class="nav__link">About Me</button>
          </li>
          <li>
            <button  class="nav__link">Experience</button>
          </li>
          <li>
            <button  class="nav__link">Portfolio</button>
          </li>
          <li>
            <button  class="nav__link">Contact</button>
          </li>
          <li>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>
<script setup>
import { ref } from "vue";
const burger = ref(false);
</script>
<style lang=""></style>
