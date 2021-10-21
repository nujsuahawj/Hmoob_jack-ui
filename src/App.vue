<template>
  <v-app>
    <Header/>
    <v-main>
      <HeroComponent/>
      <Aboutus />
      <Portfolio />
      <Project />
      <Gallery />
      <Contactus />
      <Footer />
      
    </v-main>
  </v-app>
</template>

<script>
import Header from './components/Header';
import HeroComponent from './components/HeroComponent';
import Aboutus from './components/Aboutus';
import Portfolio from './components/Portfolio';
import Project from './components/Project';
import Gallery from './components/Gallery';
import Contactus from './components/Contactus';
import Footer from './components/Footer';

export default {
  name: 'App',

  components: {
    Header,
    HeroComponent,
    Aboutus,
    Portfolio,
    Project,
    Gallery,
    Contactus,
    Footer,
  },

  data() {
    return{
      menus:[
        {title:'Home',      route:'home'},
        {title:'About us',  route:'about-us'},
        {title:'Protfolio', route:'protfolio'},
        {title:'Project',   route:'project'},
        {title:'Gallery',   route:'galley'},
        {title:'Contact',   route:'contact'},
      ]
    }
  }
};
</script>

<style>
@font-face {
  font-family: "Noto Sans Lao";
  src: local("Noto Sans Lao"),
   url(./assets/fonts/NotoSansLao-VariableFont_wdth,wght.ttf) format("truetype");
}
/* @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+Lao:wght@100&display=swap'); */
</style>
