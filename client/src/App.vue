<script setup>
import {ref} from 'vue'
let menuClass= ref("menuBar");
</script>

<template>
  <div class="home">
    <h1>Unify</h1>
  </div>
  <div :class="menuClass">
    <a href="#">Home</a>
    <a href="#">About Us</a>
    <a href="#">Contact</a>
    <a href="#">Support Us</a>
  </div>
</template>

<style lang="css">
  *{
    box-sizing: border-box; 
    margin: 0;
    padding: 0;
    border: 0;
    font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    scroll-behavior: smooth;
  }
  div.home{
    position:relative; 
    width: 100vw;
    height: 100vh;
    font-size: 2em;

    background-image: url("./assets/nightsky.png");
    background-size: cover;
    &>h1{
      position:absolute;
      color:white;
      font-size: 4em;
      left: 30px;
      bottom: 10px;
    }
  }
  div.menuBar{
    display: flex;
      flex-direction: row;
      justify-content: left;
    background-color: rgb(110, 110, 110);
    font-size:1em;
  }
  a{
    display: block;
    position: relative;
    padding: 0px 10px 0px 10px;
    background-color: rgba(255, 255, 255, 0);
    
    font-size: 2em;
    text-decoration: none;
    color:rgb(255, 255, 255);
    &:hover{
      background-color: rgba(255, 255, 255, 0.1);
    }
  }
</style>