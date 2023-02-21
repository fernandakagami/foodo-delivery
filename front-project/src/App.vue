<template>
  <Header></Header>
  
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Header from '../src/components/Header.vue'

export default defineComponent({
  name: 'App',
  components: {
    Header
  }
})
</script>

