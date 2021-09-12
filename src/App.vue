<template>
  <v-app>
  <Header/>

    <v-main>
      <HomePage/>
      <AboutAs/>
    </v-main>
  </v-app>
</template>

<script>

import HomePage from './components/homePage.vue';
import Header from './components/header.vue';
import AboutAs from './components/aboutAs.vue';

export default {
  name: 'App',

  components: {
   HomePage,
   Header,
   AboutAs
  },

  data: () => ({
   styleObject:{
    
    
   }
  }),
};
</script>
