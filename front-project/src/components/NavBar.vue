<template>
    <v-toolbar color="red-darken-1">
        <div class="v-toolbar__content">
            <v-btn color="white" to="/" class="v-toolbar__link">Find Food</v-btn>
            <v-btn color="white" to="/today-deal" class="v-toolbar__link">Today's Deal</v-btn>
        </div>
    </v-toolbar>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: "NavBar",
})
</script>

<style scoped>
.v-toolbar__content {
    display: flex;
    justify-content: center;
}

.v-toolbar__link {
    cursor: pointer;
}
</style>
