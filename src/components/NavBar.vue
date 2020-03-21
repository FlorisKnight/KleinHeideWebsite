<template>
<div class="NavBar">
  <nav>
    <div class="logo">
      <h4>Klein Heide</h4>
    </div>
    <ul class="nav-links" :class="{'nav-active': navActive}">
      <li>
        <a href="#home">Home</a>
      </li>
      <li>
        <a href="#voedselbos">Voedselbos</a>
      </li>
      <li>
        <a href="#locatie">Locatie</a>
      </li>
      <li>
        <a href="#contact">Contact</a>
      </li>
    </ul>
    <div @click="toggleMenu" class="burger">
      <div class="line1"></div>
      <div class="line2"></div>
      <div class="line3"></div>
    </div>
  </nav>
</div>
</template>

<script>

export default {
  name: 'NavBar',
  data() {
    return {
      navActive: false,
    };
  },
  methods: {
    toggleMenu() {
      this.navActive = !this.navActive;
      // some code to filter users
    },
  },
};

</script>

<style scoped>
  nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
    min-height: 8vh;
    background-color: white;
    font-family: 'Montserrat', sans-serif;
    box-shadow: 0px 2px 10px -7px rgba(0,0,0,0.12);
  }

  .logo {
    color: #1c1c1c;
    text-transform: uppercase;
    letter-spacing: 5px;
    font-size: 20px;
  }

  .nav-links {
    display: flex;
    justify-content: space-around;
    width: 50%;
  }

  .nav-links li {
    list-style: none;
  }

  .nav-links a {
    color: #1c1c1c;
    text-decoration: none;
    letter-spacing: 3px;
    font-weight: bold;
    font-size: 14px;
  }

  .burger {
    display: none;
  }

  .burger div{
    width: 25px;
    height: 3px;
    background-color: #1c1c1c;
    margin: 5px;
  }

  @media screen and (max-width: 1000px){
    .nav-links {
      position: absolute;
      right: 0px;
      height: 92vh;
      top: 8vh;
      background-color: white;
      display: flex;
      flex-direction: column;
      align-items: center;
      transform: translateX(100%);
      transition: transform 0.5s ease-in;
    }

    .nav-links li{
    }

    .burger {
      display: block;
      cursor: pointer;
    }
  }

  .nav-active{
    transform: translateX(0%);
  }
</style>
