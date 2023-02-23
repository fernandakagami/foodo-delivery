<template>
  <BannerCarousel></BannerCarousel>  
    <v-container class="d-flex flex-column justify-center align-center">      
      oi 
    </v-container>    
  
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import BannerCarousel from '../../src/components/BannerCarousel.vue'

export default defineComponent({
  name: 'HomeView',
  components: {
    BannerCarousel
  }

})
</script>

