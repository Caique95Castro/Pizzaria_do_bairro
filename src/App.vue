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
        <a
          href="https://www.instagram.com/accounts/login/"
          target="_blank"
          rel="noopener noreferrer"
          ><ion-icon class="icons-icons" name="logo-instagram"></ion-icon
        ></a>
        <a
          href="https://www.facebook.com/login/"
          target="_blank"
          rel="noopener noreferrer"
          ><ion-icon class="icons-icons" name="logo-facebook"></ion-icon
        ></a>
      </nav>
      <div class="container-menu-resp">
        <nav class="navbar">
          <a class="navbar-brand" href="/">Pizzaria do Bairro</a>
          <button
            class="navbar-toggler color-white"
            type="button"
            data-toggle="collapse"
            data-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <ion-icon class="icons-menu" name="menu-outline"></ion-icon>
          </button>

          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav mr-auto">
              <li class="nav-item active">
                <a class="nav-link" href="/"
                  >Home <span class="sr-only">(current)</span></a
                >
              </li>
              <li class="nav-item active">
                <a class="nav-link" href="/about"
                  >SOBRE NÓS <span class="sr-only">(current)</span></a
                >
              </li>
              <li class="nav-item active">
                <a class="nav-link" href="/cardapio"
                  >CARDÁPIO <span class="sr-only">(current)</span></a
                >
              </li>
              <li class="nav-item active">
                <a class="nav-link" href="/contato"
                  >CONTATO <span class="sr-only">(current)</span></a
                >
              </li>
            </ul>
          </div>
        </nav>
      </div>
    </div>
  </header>
  <router-view />
</template>
<script >
export default {
  name: "App",
};
</script>

<style lang="scss" >
@import url("https://fonts.googleapis.com/css2?family= Lato & display família= Lato:wght@400;700 & swap");
@import url("https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Indie+Flower&family=Poppins:wght@400;600;700&display=swap");

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
    margin-top: 20px;
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
.icons-icons {
  width: 20px;
  height: 20px;
}
.icons-icons:hover {
  color: rgb(251, 255, 0);
}
nav {
  a {
    font-weight: bold;
    color: white !important;
    text-decoration: none !important;

    &.router-link-exact-active {
      color: rgb(251, 255, 0) !important;
      text-decoration: underline;
    }
  }
}

.container-menu-resp {
  display: none;
}
.navbar {
  background: rgba(22, 22, 22, 0.8) !important;
}
@media (max-width: 600px) {
  .menu {
    display: none;
  }
  .logo-pizza {
    display: none;
  }
  .container-menu-resp {
    display: block;
    width: 100%;
    z-index: 400;
  }
  .header {
    display: block;
    margin-top: 0;
  }
  .nav-link {
    color: white !important;
  }
  header {
    background: transparent;
  }
  .navbar-brand a:hover  {
    color: white;
  }
  .icons-menu{
    width: 40px;
    height: 40px;
    color: white;
  }
 
  
  
}
</style>
