<template>
    <div class="d-flex justify-center align-center">
        <v-btn v-for="food in foods" :key="food.name" class="mx-5 my-16 v-btn--icon" icon>
            <img :src="food.src" class="food-category-image">
        </v-btn>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: "FoodCategory",
    data: () => ({
        foods: [
            {
                src: new URL(`../assets/foods/burger.png`, import.meta.url).href,
                name: 'Cheeseburger'
            },
            {
                src: new URL(`../assets/foods/french-fries.png`, import.meta.url).href,
                name: 'Hot Dog'
            },
            {
                src: new URL(`../assets/foods/hot-dog.png`, import.meta.url).href,
                name: 'French Fries'
            },
            {
                src: new URL(`../assets/foods/pizza.png`, import.meta.url).href,
                name: 'Pizza'
            },
            {
                src: new URL(`../assets/foods/donut.png`, import.meta.url).href,
                name: 'Donut'
            },
            {
                src: new URL(`../assets/foods/taco.png`, import.meta.url).href,
                name: 'Taco'
            },
        ],
    }),
})
</script>

<style scoped>
.v-btn--icon {
    width: 120px !important;
    height: 120px !important;
}

.food-category-image {
    width: 80px;
}
</style>
