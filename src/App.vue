<template>
 <section>
   <Navbar />
  <router-view/>
  
  <Footer />
 </section>
</template>

<script>
  import Navbar from './components/Navbar.vue'
  import Footer from './components/Footer.vue'

export default {
  components : {
    Navbar,
    Footer
  }
}
</script>

<style>

 @font-face {
    font-family: 'DinNextLight';
    src: url('./assets/fonts//din-next/light/DinNextLight.eot');
    src: url('./assets/fonts/din-next/light/DinNextLight.eot') format('embedded-opentype'), url('./assets/fonts/din-next/light/DinNextLight.woff2') format('woff2'), url('./assets/fonts/din-next/light/DinNextLight.woff') format('woff'), url('./assets/fonts/din-next/light/DinNextLight.ttf') format('truetype'), url('./assets/fonts/din-next/light/DinNextLight.svg#DinNextLight') format('svg');

  }
  @font-face {
    font-family: 'DinNextRegular';
    src: url('./assets/fonts/din-next/regular/DinNextRegular.eot');
    src: url('./assets/fonts/din-next/regular/DinNextRegular.eot') format('embedded-opentype'), url('./assets/fonts/din-next/regular/DinNextRegular.woff2') format('woff2'), url('./assets/fonts/din-next/regular/DinNextRegular.woff') format('woff'), url('./assets/fonts/din-next/regular/DinNextRegular.ttf') format('truetype'), url('./assets/fonts/din-next/regular/DinNextRegular.svg#DinNextRegular') format('svg');
}

@font-face {
    font-family: 'DinNextBold';
    src: url('./assets/fonts/din-next/bold/DinNextBold.eot');
    src: url('./assets/fonts/din-next/bold/DinNextBold.eot') format('embedded-opentype'), url('./assets/fonts/din-next/bold/DinNextBold.woff2') format('woff2'), url('./assets/fonts/din-next/bold/DinNextBold.woff') format('woff'), url('./assets/fonts/din-next/bold/DinNextBold.ttf') format('truetype'), url('./assets/fonts/din-next/bold/DinNextBold.svg#DinNextBold') format('svg');
}

:root {
  font-size: 18px;
}

@media (max-width: 900px) {
  :root {
    font-size: 13px;
  }
}

@media (max-width: 700px) {
  :root {
    font-size: 8px;
  }
}

*{
    font-family: 'DinNextRegular';
}


</style>
