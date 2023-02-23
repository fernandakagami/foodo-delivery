<template>
    <BannerCarousel></BannerCarousel>
    <FoodCategory></FoodCategory>
    <v-container>
        <v-row>
            <v-col cols="3" v-for="restaurant in restaurants" :key="restaurant.name">
                <v-card class="pa-6" to="#">
                    <v-img :src="restaurant.src" class="restaurant-logo"></v-img>
                    <v-card-title class="text-center">{{ restaurant.name }}</v-card-title>
                    <v-card-subtitle class="px-0 pb-1"><strong>&#9733;</strong> {{ restaurant.star }} &#x2022; {{ restaurant.type }}</v-card-subtitle>
                    <v-card-subtitle class="px-0">{{ restaurant.time[0] }}-{{ restaurant.time[1] }} min &#x2022; {{ restaurant.distance }}km &#x2022; {{ restaurant.delivery ? `R$ ${restaurant.delivery}` : 'Grátis' }}</v-card-subtitle>
                </v-card>
            </v-col>
        </v-row>
    </v-container>
</template>

<script lang="ts">
import FoodCategory from '@/components/FoodCategory.vue'
import { defineComponent } from 'vue'
import BannerCarousel from '../../src/components/BannerCarousel.vue'

export default defineComponent({
    name: 'HomeView',
    components: {
        BannerCarousel,
        FoodCategory
    },
    data: () => ({
        restaurants: [
            {
                src: new URL(`../assets/restaurants/01.png`, import.meta.url).href,
                name: 'Cheeseburger',
                star: 4.4,
                type: 'Cheeseburger',
                distance: 4.0,
                time: [29, 39],
                delivery: 12.99

            },
            {
                src: new URL(`../assets/restaurants/02.png`, import.meta.url).href,
                name: 'French Fries',
                star: 4.9,
                type: 'French Fries',
                distance: 0.9,
                time: [23, 33],
                delivery: ''
            },
            {
                src: new URL(`../assets/restaurants/03.png`, import.meta.url).href,
                name: 'Hot Dog',
                star: 4.1,
                type: 'Hot Dog',
                distance: 1.2,
                time: [40, 50],
                delivery: 7.00
            },
            {
                src: new URL(`../assets/restaurants/03.png`, import.meta.url).href,
                name: 'Hot Dog',
                star: 4.1,
                type: 'Hot Dog',
                distance: 1.2,
                time: [40, 50],
                delivery: 7.00
            },
        ],
    }),
})
</script>

<style scoped>

.restaurant-logo {
    max-width: 100%;
}

strong {
    color: rgb(228, 228, 12);
}
</style>