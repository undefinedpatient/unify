<script setup>
import {ref} from 'vue'
let menuClass= ref("menuBar");
</script>

<template>
  <div class="home">
    <h1>Vertex Studio</h1>
    
  </div>
  <div :class=menuClass>
    <a href="#">Home</a>
    <a href="#aboutUs">About Us</a>
    <a href="#">News</a>
    <a href="#">Contact</a>
    <a href="#">Support Us</a>
  </div>
  <div class="aboutUs" id="aboutUs">
    <h2>About Us</h2>
    <p>
      Welcome to Vertex, an indie animation studio crafting vibrant, 
      heartfelt stories that captivate and inspire. With a passionate team of artists and storytellers, 
      we blend innovative techniques with timeless narratives to create unique animated experiences. 
      From whimsical shorts to bold feature films, our work celebrates creativity and connection. 
      Join us on this colorful journey!
    </p>
  </div>
  <div class="news" id="news">
    <h2>News</h2>
    <p>
    </p>
  </div>
  <div class="contacts" id="contacts">
    <h2>Contacts</h2>
    <p>
    </p>
  </div>
  <div class="supportUs" id="supportUs">
    <h2>Support Us</h2>
    <p>
    </p>
  </div>
  <footer>
    <p>&copy; 2025 Vertex. All rights reserved.</p>
    <div class="contact-links">|
      <a href="#">contact@gmail.com</a> |
      <a href="#">+852 1234 5678</a> |
      <a href="#">Discord</a> |
      <a href="#">X</a> |
    </div>
  </footer>
</template>

<style lang="css">
  div.home{
    position:relative; 
    width: 100vw;
    height: 100vh;
    font-size: 2em;
    
    background-image: url("./assets/nightsky.png");
    background-size: cover;
    &>h1{
      position:absolute;
      left: 32px;
      bottom: 72px;
    }
  }
  div.menuBar{
    position:sticky;
    display: flex;
      flex-direction: row;
      justify-content:left;
    z-index: 1;
    top: 0;
    margin: -60px 0 0 0;
    background-color: rgba(0, 0, 0, 0.4);
    font-size: 2em;
    width: 100vw;
    height: 60px;
    & a{
      display: block;
      position: relative;
      padding: 8px 24px 8px 24px;
      background-color: rgba(255, 255, 255, 0);
      min-width: max-content;
      overflow: hidden;
      font-size: 100%;
      text-decoration: none;
      &:hover{
        background-color: rgba(255, 255, 255, 0.1);
      }
    }
  }
  div.aboutUs{
    position: relative;
    display: block;
    width: 100vw;
    height: max-content;
    padding: 64px;
    font-size: 1rem;
    background-color: var(--layer00);
    background-image: 
    linear-gradient(0deg,rgba(24, 24, 24, 0.8),50%, rgba(20, 20, 20, 0.5)),
    url("./assets/studio.png");
      
    background-size: cover;
    & p{
      font-size: 1em;
      max-width: 800px;
    }
    
  }
  div.news{
    position: relative;
    display: block;
    width: 100vw;
    height: max-content;
    padding: 64px;
    font-size: 1rem;
    background-color: var(--layer01);
  }
  div.contacts{
    position: relative;
    display: block;
    width: 100vw;
    height: max-content;
    padding: 64px;
    font-size: 1rem;
    background-color: var(--layer01);
  }
  div.supportUs{
    position: relative;
    display: block;
    width: 100vw;
    height: max-content;
    padding: 64px;
    font-size: 1rem;
    background-color: var(--layer01);
  }
  footer{
    position:relative;
    display: flex;
      flex-direction: row;
      justify-content: space-between;
    background-color: var(--layer00);
    color: #ecf0f1;
    font-style: italic;
    padding: 20px;
    width: 100%;
    & p{
      color: #ecf0f1;
    }
    & .contact-links a{
      text-decoration: none;
    }
  }
  @media (min-width: 600px) {
    
  }

</style>