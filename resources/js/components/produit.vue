<template>
    <div class="produit">
        <div class="flex flex-row justify-between mx-28">
            <!-- <input type="text" class="ring-1 rounded-xl p-2" placeholder="Recherche"> -->
            <div class="font-bold"> Produits </div>
            <button  class="shadow-xl text-white bg-blue-400 w-24 h-12 rounded-2xl font-bold"  @click="addArticle"> Ajouter </button>
        </div>
       
        <!-- <div v-show="produits">  lksjfkdsjmfsdkflsdfkdsmkjfdsqklmfjsqfjklmdskmlklmsdklfjsdlkf </div> -->
        <Article v-show="!produits"/>
        <AddArticle v-show="add"/>
    </div>
</template>

<script>
import Article from './Articles.vue'
import AddArticle from './pages/Addarticle.vue'
    export default {
        name:"produit",
        components: {
            Article,
            AddArticle
        },
        data() {
            return {
                produits: false,
                add: false
            }
        },
        methods: {
            // toAddArt() {
                
            // },
            addArticle() {
                this.$router.push({ name: 'Addarticle' })
            }
        },
        mounted() {
            localStorage.getItem('page', 'products')
        },
        computed:{
            filter(produit){
                return this
            }
        }
    };
</script>

<style lang="scss" scoped>

</style>