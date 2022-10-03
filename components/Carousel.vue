<template>
    <div class="bg">
        <div class="row justify-center my-10 pa-2">
            <div>
                <div id="font" class="text-h4 white--text text-uppercase text-center pa-4">Galerie</div>
                <div class="text-subitle white--text text-center pa-4">Notre établisement en photos</div>
                <div class="row justify-center pa-2 fill-height">
                    <div class="col-md-8 col-12 mx-auto">
                        <v-carousel>
                            <v-carousel-item v-for="(item,i) in items" :key="i" :src="item.src"
                                reverse-transition="fade-transition" transition="fade-transition"></v-carousel-item>
                        </v-carousel>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            items: [
                {
                    src: 'https://images.unsplash.com/photo-1664627206290-9a9877f81da3?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1740&q=80',
                },
                {
                    src: 'https://images.unsplash.com/photo-1664447972862-e26efc5b709f?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1932&q=80',
                },
                {
                    src: 'https://images.unsplash.com/photo-1664663751485-c58e9276ccce?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1734&q=80',
                },
            ]
        }
    }
}
</script>

<style scoped>
.bg {
    background-image: linear-gradient(rgba(122, 11, 28, 0.7), rgba(122, 11, 28, 0.7)), url("https://lespelette-reims.fr/main.avif");
    background-position: center center;
    background-size: cover;
    height: 700px;
}

#font {
    font-family: 'Bree Serif', serif !important;
}
</style>