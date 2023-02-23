<template>
  <Header></Header>
  <NavBar></NavBar>  
  <RouterView />
  <Footer></Footer>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Header from '../src/components/Header.vue'
import NavBar from '../src/components/NavBar.vue'
import Footer from '../src/components/Footer.vue'

export default defineComponent({
  name: 'App',
  components: {
    Header,
    NavBar,
    Footer
  }
})
</script>

