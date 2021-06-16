<template>
    <div  class="modproduit">
       <!-- <form @submit="updateProduit"> -->
           <div v-for="produit in produits" :key="produit.id">
               <div class="flex flex-col" >
                    <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="Nom" v-model="produit.nom">
                    <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="categorie" v-model="produit.categorie">
                    <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="prix" v-model="produit.prix">
                    <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="quantité" v-model="produit.quantite">
                    <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="image" v-model="produit.image">
                    <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="description" v-model="produit.description">
                </div>
        <button class="bg-gray-600 p-2 rounded-full" @click="updateProduit(produit)"> Enregistrer </button>
           </div>
       <!-- </form> -->
    </div>
</template>
<script>
import axios from 'axios'
export default {
    name: 'Modproduit',
    data() {
        return {
            selectedFile: null,
            produits: []
        }
    },
    created() {
        this.getProduits()
    },
    methods: {
        getProduits() {
            axios.get(`produits/${localStorage.getItem('id')}`)
            .then((response) => {
                this.produits = response.data
            })
        },
        updateProduit(produit) {
            axios.put(`produit/${localStorage.getItem('id')}`, {
                nom: produit['nom'],
                categorie: produit['categorie'],
                prix: produit['prix'],
                quantite: produit['quantite'],
                image: produit['image'],
                desciption: produit['description'],
                commande_confirme: 'no'
            }).then(() => {
                // console.log('updated');
                this.$router.push({ name: 'Dashboard' })
                
            })
        }
        // addArt() {
        //     axios.post('produit', {
        //         nom: this.nom,
        //         categorie: this.categorie,
        //         prix:  this.prix,
        //         quantite:  this.quantite,
        //         image:  this.image,
        //         description:  this.description,
        //         reviews: 3,
        //         commande_confirme: 'no'
        //     })
        //     .then(() => {
        //         console.log('Success');
        //         localStorage.setItem('page', 'products')
        //         this.$router.push({ name: 'Dashboard' })
        //     }).catch((e) => {
        //         console.log(e);
        //     })
        // },
        // onChange(e) {
        //     // if(this.selectedFile)
        //         this.file = e.target.files[0]
                
        // },
        // formSubmit(e) {
        //     e.preventDefault();
        //     let existingObj = this;

        //     const config = {
        //         headers: {
        //             'content-type': 'multipart/form-data'
        //         }
        //     }

        //     let data = new FormData();
        //     data.append('file', this.file)
        //     data.append('nom', this.nom)
        //     data.append('categorie', this.categorie)
        //     data.append('prix', this.prix)
        //     data.append('image', this.image)
        //     data.append('description', this.description)
        //     data.append('reviews', 3)
        //     data.append('commande_confirme', 'no')

        //     axios.post('produit', this.data)
        //     .then((res) => {
        //         existingObj.success = res.data.success
        //     })
        // }
    }
}
</script>

<style lang="scss" scoped>

</style>