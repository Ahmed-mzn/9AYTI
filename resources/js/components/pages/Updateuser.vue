<template>
    <div  class="updateuser">
       <!-- <form @submit="updateuser"> -->
           <div v-for="user in users" :key="user.id">
               <div class="flex flex-col" >
                    <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="Nom" v-model="user.name">
                    <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="Email" v-model="user.email">
                    <input class="rounded-full bg-white ring-1 w-64 h-12 p-2 mb-2" placeholder="password" v-model="user.password">

                </div>
        <button class="bg-gray-600 p-2 rounded-full" @click="updateUser(user)"> Enregistrer </button>
           </div>
       <!-- </form> -->
    </div>
</template>
<script>
import axios from 'axios'
export default {
    name: 'Updateuser',
    data() {
        return {
            selectedFile: null,
            users: [],
            user: ''
        }
    },
    created() {
        this.getusers()
    },
    methods: {
        getusers() {
            axios.get(`user/${localStorage.getItem('id')}`)
            .then((response) => {
                this.users = response.data
                console.log(this.users);
                
            })
        },
        updateUser(user) {
            axios.put(`user/${localStorage.getItem('id')}`, {
                name: user['name'],
                email: user['email'],
                password: user['password'],
            }).then(() => {
                this.$router.push({ name: 'Dashboard' })
                
            })
        }
      
    },
    mounted() {
        this.user = (localStorage.getItem('id'))
        // console.log(this.user);
        
    },
}
</script>

<style lang="scss" scoped>

</style>