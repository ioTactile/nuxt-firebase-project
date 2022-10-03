<template>
    <v-app-bar color="surface" flat>

        <NuxtLink to="/"><img src="~assets/img/logo.png" width="60" /></NuxtLink>

        <div class="spacer"></div>

        <v-btn v-for="button in buttons" :key="button.id" :to="button.redirection" class="bg--text" color="surface"
            height="inherit" tile depressed>
            <span>{{button.name}}</span>
        </v-btn>

    </v-app-bar>
</template>

<script>
export default {
    data() {
        return {
            buttons: [
                {
                    name: 'Accueil',
                    redirection: '/',
                },
                {
                    name: 'À propos',
                    redirection: '/presentation'
                },
                {
                    name: 'La carte',
                    redirection: '/carte'
                },
                {
                    name: 'Actualités',
                    redirection: '/blog'
                },
                {
                    name: 'Contact',
                    redirection: 'contact'
                },
            ]
        }
    }
}
</script>

<style scoped>
img {
    margin-top: 0.5rem;
}

.spacer {
    flex-grow: 1;
}
</style>