<template>
    <v-layout class="footer-container">
        <div class="d-flex flex-column">
            <v-btn color="red-darken-1" class="mb-16 mx-16" size="large">Contact Us</v-btn>

            <div class="mb-10">
                <v-btn v-for="link in links" :key="link" variant="text" class="mx-2" rounded="xl">
                    {{ link }}
                </v-btn>
            </div>

            <p class="mb-7 text-center">© {{ new Date().getFullYear() }} <strong>Foodo</strong>. All rights reserved.</p>
        </div>
    </v-layout>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: "Footer",
    data: () => ({
        links: [
            'Home',
            'About Us',
            'Team',
            'Services'
        ],
    }),
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