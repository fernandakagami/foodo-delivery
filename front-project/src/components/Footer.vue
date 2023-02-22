<template>
    <v-container class="footer-container">        
        <p>© {{ new Date().getFullYear() }} <strong>Foodo</strong>. All rights reserved.</p>        
    </v-container>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: "Footer"
})
</script>

<style scoped>
.footer-container {    
    display: flex;
    height: 500px;
    justify-content: center;
    align-items: end;
    background: url(https://cdn.shopify.com/s/files/1/0740/5717/files/leo_foodo_bg-footer-ldp.jpg?v=1603334708) no-repeat 0 0 #fff;
}
</style>