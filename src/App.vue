<template>
  <header>
    <div class="header">
      <div class="logo-pizza">
        <!-- <img class="pizza" src="#" alt=""> -->
        <h1 class="logo">Pizzaria do Bairro</h1>
      </div>
      <nav class="menu">
        <router-link to="/">HOME</router-link>
        <router-link to="/about">SOBRE NÓS</router-link>
        <router-link to="/cardapio">CARDÁPIO</router-link>
        <router-link to="/contato">CONTATO</router-link>
        <a href="https://www.instagram.com/accounts/login/" target="_blank" rel="noopener noreferrer"
            ><ion-icon class="icons-icons" name="logo-instagram"></ion-icon
          ></a>
          <a href="https://www.facebook.com/login/" target="_blank" rel="noopener noreferrer"
            ><ion-icon class="icons-icons" name="logo-facebook"></ion-icon
          ></a>
      </nav>
    </div>
  </header>
  <router-view />
</template>

<style lang="scss" >
@import url('https://fonts.googleapis.com/css2?family= Lato & display família= Lato:wght@400;700 & swap');
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Indie+Flower&family=Poppins:wght@400;600;700&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
}
header {
  position: fixed;
  width: 100%;
  background: rgba(22, 22, 22, 0.8);
  z-index: 200;
}
.header {
  text-transform: uppercase;
  height: 100px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  text-align: center;
  font-size: 1rem;
}
@media screen and (max-width: 1000px) {
  .header {
    text-transform: uppercase;
    height: 100px;
    display: flex;
    flex-direction: column;
    font-size: 1rem;
  }
}
.logo-pizza {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
}
.pizza {
  width: 100px;
  height: 100px;
}
.logo {
  font-size: 1.2rem;
  letter-spacing: 0.4rem;
  color: white;
}

.menu {
  display: flex;
  gap: 20px;
}
.icons-icons{
  width: 20px;
  height: 20px;
}
.icons-icons:hover{
  color: rgb(251, 255, 0);
}
nav {
  a {
    font-weight: bold;
    color: white;
    text-decoration: none;

    &.router-link-exact-active {
      color: rgb(251, 255, 0);
      text-decoration: underline;
    }
  }
}
</style>
