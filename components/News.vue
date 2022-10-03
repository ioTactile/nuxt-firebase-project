<template>
    <div class="my-6" style="margin-right: auto; margin-left: auto; max-width: 1185px;">
        <div class="row justify-center">
            <span id="font" class="text-center text-uppercase text-h4 my-6">actualites</span>
        </div>
        <div class="row justify-center">
            <div v-for="(blog,i) in blogs" :key="i" class="col-md-4 col-12 ">
                <a class="mx-auto" href="/blog" style="text-decoration:none;">
                    <div :style="blog.image"
                        style="background-position:center center; background-size: cover; height: 250px; width:auto;">
                        <div class="text-center white--text">
                            <div class="col col-12" style="background-color:#7A0B1C; opacity:0.9; ">
                                <span id="font" class=" text-h6 text-uppercase font-weight-bold">{{blog.text}}</span>
                            </div>
                        </div>
                    </div>
                </a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            blogs: [
                {
                    text: 'Les rhums de l\'espelette',
                    image: {
                        backgroundImage: "url(https://images.unsplash.com/photo-1597290282695-edc43d0e7129?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1750&q=80)",
                    }
                },
                {
                    text: 'Elles font leur retour dans vos assiettes',
                    image: {
                        backgroundImage: "url(https://images.unsplash.com/photo-1504674900247-0877df9cc836?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1740&q=80)",
                    }
                },
            ]
        }
    }
}
</script>

<style scoped>
#font {
    font-family: 'Bree Serif', serif !important;
}
</style>

