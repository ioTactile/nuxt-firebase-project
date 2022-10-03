<template>
    <div class="bg">
        <div class="row align-center justify-center white--text pa-2 fill-height">
            <div class="col-md-8 col-12 text-center mx-auto ">
                <div class="logo mb-8"></div>
                <h1 id="font" class="text-uppercase font-weight-bold text-h3">* L'espelette *</h1>
                <h2 id="font" class="text-h5 mt-10">Spécialités basques et espagnoles - Bar à tapas</h2>
            </div>
            <div class="col col-8">
                <div class="row justify-center">
                    <div class="col-md-4 col-12">
                        <div class="text-center">
                            <v-btn class="white--text" outlined href="tel: 03 00 00 00 00"><span>Réserver</span></v-btn>
                        </div>
                    </div>
                    <div class="col-md-4 col-12">
                        <div class="text-center">
                            <v-btn class="white--text" color="bgdark" to="/presentation"><span>Nous découvrir</span>
                            </v-btn>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<style scoped>
.bg {
    background-image: linear-gradient(rgba(122, 11, 28, 0.7), rgba(122, 11, 28, 0.7)), url("https://lespelette-reims.fr/main.avif");
    background-position: center center;
    background-size: cover;
    height: 500px;

}

.logo {
    background-image: url("https://lespelette-reims.fr/logo.svg");
    background-position: center center;
    height: 190px;
}

#font {
    font-family: 'Bree Serif', serif !important;
}
</style>
