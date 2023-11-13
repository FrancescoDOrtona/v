<template>
    <nav class="navbar">
        <div class="header">
            <ul class="menu">
                <li v-for="(gender, index) in genders"> <a href="#">{{ gender }}</a></li>   
            </ul>
            <img class="logo" src="../assets/boolean-logo.png" alt="">
            <div class="icons">
                <a href=""><font-awesome-icon icon="fa-regular fa-user" /></a>
                <a href=""><font-awesome-icon icon="fa-regular fa-heart" /></a>
                <a href=""><font-awesome-icon icon="fa-solid fa-bag-shopping" /></a>
            </div>
        </div>       
    </nav>
    
  </template>
  
  <script>
  
    export default {
      data() {
        return {
            genders: ['Donna', 'Uomo', 'Bambino']
        }
      }
    }
  </script>
  
  <style lang="scss" scoped>
  @use '../styles/partials/variables' as *;

  .navbar{
    background-color: $main-color;
    width: 100%;
    box-shadow: 0px 0px 5px 0px black;
    position: fixed;
    left: 0;
    right: 0;
    top: 0;
    z-index: 100;
  }

  .header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px;
  }
  .menu {
    display: flex;
    gap: 15px;
  }

  .logo{
    width: 150px;
    justify-content: center;
  }

  .icons{
    display: flex;
    align-items: center;
    gap: 15px;

  }
  </style>