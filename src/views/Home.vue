<template>
  <div class="home">
    <NavBar class="Navigation"></NavBar>
    <div class="itemBoxes">
      <header class="header-box" id="home">
        <img class="header-logo" src="../assets/img/Frog.png"/>
        <h1 class="header-text">Klein Heide</h1>
      </header>
      <Voedselbos id="voedselbos"></Voedselbos>
      <PictureCarousel></PictureCarousel>
      <PictureDivider :url="require('../assets/img/pink-flower.jpg')"></PictureDivider>
      <Locatie id="locatie"></Locatie>
      <PictureDivider :url="require('../assets/img/pink-flower.jpg')"></PictureDivider>
      <Contact id="contact"></Contact>
      <FooterComp></FooterComp>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '../components/NavBar.vue';
import Voedselbos from '../components/Voedselbos.vue';
import Locatie from '../components/Locatie.vue';
import Contact from '../components/Contact.vue';
import PictureDivider from '../components/PictureDivider.vue';
import FooterComp from '../components/FooterComp.vue';
import PictureCarousel from '../components/PictureCarousel.vue';

export default {
  name: 'home',
  components: {
    PictureCarousel,
    FooterComp,
    PictureDivider,
    Contact,
    Locatie,
    Voedselbos,
    NavBar,
  },
};
</script>

<style scoped>
  .Navigation {
    position: fixed;
    width: 100%;
  }
  .itemBoxes {
    padding-top: 8vh;
  }
  .header-box {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 10vh;
    background-image: linear-gradient(
      120deg,
      rgba(212, 252, 121, 1) 0%,
      rgba(150, 230, 161, 1) 100%);
  }
  .header-logo {
    width: 40%;
    max-width: 400px;
  }
  .header-text {
    font-family: 'Montserrat', sans-serif;
    text-transform: uppercase;
    letter-spacing: 5px;
    font-size: 1.3rem;
  }
</style>
