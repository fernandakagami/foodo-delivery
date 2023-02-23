<template>
    <v-carousel height="550" cycle show-arrows="hover">
        <v-carousel-item v-for="(item, i) in items" :key="i">
            <img :src="item.src" style="width:100%;height:100%;" :alt="`banner${i}`"/>
        </v-carousel-item>
    </v-carousel>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: "BannerCarousel",
    data() {
        return {
            items: [
                {
                    src: new URL(`../assets/banners/banner00.png`, import.meta.url).href,
                },
                {
                    src: new URL(`../assets/banners/banner01.png`, import.meta.url).href,
                },
                {
                    src: new URL(`../assets/banners/banner02.png`, import.meta.url).href,
                },              
            ],
        }
    },
})
</script>

<style scoped>
.v-carousel-item {
    cursor: pointer;
}
</style>