<template>
    <header>
        <div>
            <img src="./icons/logo.png" alt="Foodo Delivery Logo">
            <h1>Foodo Delivery</h1>
        </div>
        <div>
            <v-text-field label="Search for restaurant..."></v-text-field>
            <v-btn size="large" color="red-darken-1">Search</v-btn>
        </div>
        <div>
            <v-icon color="success" icon="mdi-information" size="large"></v-icon>
            My Account
            Sign in - Register
        </div>
    </header>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: "Header"
})
</script>

