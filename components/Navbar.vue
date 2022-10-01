<template>
    <v-app-bar color="surface">

        <NuxtLink to="/"><img src="~assets/img/logo.png" width="60" /></NuxtLink>
        <div class="spacer"></div>
        <v-btn class="bg--text" color="surface" height="inherit" to="/" tile depressed><span>Accueil</span></v-btn>
        <v-btn class="bg--text" color="surface" height="inherit" to="/presentation" tile depressed><span>À
                propos</span></v-btn>
        <v-btn class="bg--text" color="surface" height="inherit" to="/carte" tile depressed><span>La carte</span>
        </v-btn>
        <v-btn class="bg--text" color="surface" height="inherit" to="/blog" tile depressed><span>actualités</span>
        </v-btn>
        <v-btn class="bg--text" color="surface" height="inherit" to="/contact" tile depressed><span>Contact</span>
        </v-btn>
    </v-app-bar>
</template>

<style>
img {
    margin-left: 0.5rem;
    margin-top: 0.5rem;
}

.spacer {
    flex-grow: 1;
}
</style>