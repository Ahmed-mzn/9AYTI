<template>
    <div  class="Addarticle">
       <form @submit="formSubmit">
           <div class="flex flex-col">
                <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="Nom" v-model="nom">
                <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="categorie" v-model="categorie">
                <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="prix" v-model="prix">
                <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="quantité" v-model="quantite">
                <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="image" type="file" v-on:change="onChange">
                <!-- <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="image" v-model="image"> -->
                <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="description" v-model="description">
            </div>
       <button class="bg-gray-600 p-2 rounded-full"> Enregistrer </button>
       </form>
    </div>
</template>
<script>
import axios from 'axios'
export default {
    name: 'Addarticle',
    data() {
        return {
            selectedFile: null,
            file: '',
            nom: '',
            categorie: '',
            prix: '',
            quantite: '',
            image: '',
            description: '',
        }
    },
    methods: {
        addArt() {
            axios.post('produit', {
                nom: this.nom,
                categorie: this.categorie,
                prix:  this.prix,
                quantite:  this.quantite,
                image:  this.image,
                description:  this.description,
                reviews: 3,
                commande_confirme: 'no'
            })
            .then(() => {
                console.log('Success');
                localStorage.setItem('page', 'products')
                this.$router.push({ name: 'Dashboard' })
            }).catch((e) => {
                console.log(e);
            })
        },
        onChange(e) {
            // if(this.selectedFile)
                this.file = e.target.files[0]
                // console.log(this.file);
                
                
        },
        formSubmit(e) {
            e.preventDefault();
            let existingObj = this;

            const config = {
                headers: {
                    'content-type': 'multipart/form-data'
                }
            }

            let data = new FormData();
            data.append('file', this.file)
            data.append('nom', this.nom)
            data.append('categorie', this.categorie)
            data.append('prix', this.prix)
            data.append('quantite', this.quantite)
            data.append('image', this.image)
            data.append('description', this.description)
            data.append('reviews', 3)
            data.append('commande_confirme', 'no')

            // console.log(data);
            

            axios.post('produit', data, config)
            .then((res) => {
                // existingObj.success = res.data.success
                this.$router.push({ name: 'Dashboard' })
                // console.log('you');
                
            })
        }
    }
}
</script>

<style lang="scss" scoped>

</style>