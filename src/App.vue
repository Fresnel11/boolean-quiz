<script setup>
import { RouterLink, RouterView } from 'vue-router'
import quizzArea from "./components/quizzArea.vue";

</script>

<template>
  <div>
    <nav>
      <ul>
        <li><a href=""><img class="img" src="../public/Boolean-removebg-preview.png" alt="Boolean Quiz"></a></li>
        <li class="middle"><a href="">Informatique générale</a></li>
        <li class="dev"><a href="">Informatique dev</a></li>
      </ul>
    </nav>
    <quizzArea />
    <RouterView />

   
  </div>
  
</template>

<style scoped>
  
  a {
    color: inherit;
    text-decoration: none
  }

  nav li.middle {
  margin-left: auto;
  margin-right: -15rem; /* Ajustez cette valeur comme vous le souhaitez */
}

  li {
    list-style: none;
  }

  nav li:first-child {
    margin-right: auto;
  }

 .img {
    width: 200px;
    height: auto;
 }

 nav {
  position: sticky;
  top: 0;
  left: 0;
  width: 100%;
  padding: 25px;
 }

  nav li:not(:first-child) {
    margin-left: auto;
  }

  ul {
    align-items: center;
    display: flex;
    justify-content: space-between;
    padding: 0;
    margin: 0;
  }

  nav {
    background-color: white;
    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  }

  .dev {
    margin-right: 5rem;
  }
  

</style>
