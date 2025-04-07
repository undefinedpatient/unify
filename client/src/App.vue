<script setup>
import {ref} from 'vue'
let menuClass= ref("menuBar");
</script>

<template>
  <div>Unify</div>
  <div v-bind:class="menuClass">
    <a href="">Home</a>
    <a href="">About Us</a>
    <a href="">Contact</a>
    <a href="">Support Us</a>
  </div>
</template>

<style lang="css">
  div{
    font-size: 2em;
  }
  div.menuBar{
    font-size:1em;
  }
</style>