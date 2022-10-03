<template>
    <div class="row mt-8 pb-3" style="max-width:1185px; margin-right:auto; margin-left:auto">
        <div class="col col-12">
            <div>
                <div class="text-center">
                    <v-btn class="mb-3" outlined x-large color="surface" href="tel: 03 00 00 00 00"><span>Réserver une
                            table</span>
                    </v-btn>
                </div>
                <div class="row align-center justify-center pb-5">
                    <div class="col-md-7 col-12">
                        <div class="map" style="height: 400px"></div>
                    </div>
                    <div class="font-weight-bold col-md-5 col-12">
                        <span class="mr-5" style="font-size:60px; color:#7A0B1C">X</span>
                        <a class="black--text text-decoration-none text-h6"
                            href="https://google.fr/maps/place/29 Rue Roger Salengro 51100 Reims" target="_blank">29 Rue
                            Roger Salengro 51100 Reims</a>
                        <br />
                        <span class="mr-5" style="font-size:60px; color:#7A0B1C">X</span>
                        <a class="black--text text-decoration-none text-h6" href="tel:03 26 87 50 52" target="_blank">03
                            26 87
                            50 52</a>
                    </div>
                </div>
                <v-divider></v-divider>
                <div id="font" class="text-center text-uppercase text-h4 py-5">Horaires</div>
                <div v-for="horaire in horaires" :key="horaire.id"
                    class="row font-weight-bold text-center justify-center">
                    <div class="col-md-1 col-4">{{horaire.jour}}</div>
                    <div class="col-md-4 col-8">{{horaire.heures}}</div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default ({
    data() {
        return {
            horaires: [
                {
                    jour: 'Lundi',
                    heures: '12:00-14:00, 19:00-22:00',
                },
                {
                    jour: 'Mardi',
                    heures: '12:00-14:00, 19:00-22:00',
                },
                {
                    jour: 'Mercredi',
                    heures: '12:00-14:00, 19:00-22:00',
                },
                {
                    jour: 'Jeudi',
                    heures: '12:00-14:00, 19:00-22:00',
                },
                {
                    jour: 'Vendredi',
                    heures: '12:00-14:00, 19:00-23:00',
                },
                {
                    jour: 'Samedi',
                    heures: '19:00-23:00',
                },
                {
                    jour: 'Dimanche',
                    heures: 'Fermé',
                }
            ]
        }
    }
})
</script>

<style scoped>
#font {
    font-family: 'Bree Serif', serif !important;
}

.map {
    background-image: url("https://images.unsplash.com/photo-1502920514313-52581002a659?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1734&q=80");
    background-position: center center;
}
</style>
