<template>
    <div class="white--text flex text-center" style="background-color:#972b31">
        <div>
            <v-btn v-for="button in buttons" :key="button.id" :to="button.redirection" class="white--text mt-2"
                color="footerbtn" rounded depressed>
                <span>{{button.name}}</span>
            </v-btn>
        </div>
        <div style="height:68px"></div>
        <v-divider light></v-divider>
        <div class="white--text py-4" style="font-size:14px">2022 - Made with love by <strong>
                <a class="white--text" style="text-decoration:none" href="https://nutab.fr/">NUTAB</a>
            </strong></div>
    </div>
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
                    redirection: '/contact'
                },
                {
                    name: 'Mentions légales',
                    redirection: '/mentions-legales'
                },
            ]
        }
    }
}
</script>

<style scoped>

</style>