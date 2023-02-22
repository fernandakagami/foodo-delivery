<template>    
        <v-toolbar color="white" class="my-2 py-5" height="100px" cols="6" offset="3">
            <v-row justify="space-between" align="center">
                <v-col md="3" class="d-flex justify-center align-end pa-0">
                    <div class="logo">
                        <img src="./icons/logo.png" alt="Foodo Delivery Logo">
                    </div>                    
                    <h1 class="text-h3"><small class="text-h2">F</small>oodo</h1>
                </v-col>
                
                <v-col md="6" class="d-flex justify-center align-center">
                    <v-text-field label="Search for restaurant..." hide-details class="mr-2" append-inner-icon="mdi-magnify" variant="solo" density="compact"></v-text-field>                    
                    <v-btn variant="elevated" color="red-darken-1">Search</v-btn>                    
                </v-col>
                
                <v-col md="3" class="d-flex justify-center align-center">
                    <v-icon color="red-darken-1 mr-2" icon="mdi-account-outline" size="x-large"></v-icon>
                    <div class="d-flex flex-column">
                        <v-btn href="#" variant="flat" size="small" class="link px-0">My Account</v-btn>
                        <v-btn href="#" variant="flat" size="small" class="link px-0">Sign in - Register</v-btn>
                    </div>
                </v-col>
            </v-row>
        </v-toolbar>
    
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: "Header"
})
</script>

<style scoped>
@import '../assets/base.css';

.logo img {
    width: 90px;
}

h1 {
    font-family: 'Sacramento', cursive !important;
    font-weight: 550;    
}

small {
    font-family: 'Sacramento', cursive !important;
    color: #E53935;
    font-weight: 900;
}

.link {
    color: --vt-c-indigo !important;
    --v-btn-height: 20px;
}
</style>

