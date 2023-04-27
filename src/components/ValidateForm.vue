<template>
    <div class="w-[90%] mx-auto py-20"> 
        <div class="flex"> 
            <div class="bg-white w-[90%] h-[720px] mx-auto shadow-md rounded-l-lg">
                <h2 class="bg-pink-600 text-2xl py-4 text-white text-center rounded-l-lg font-bold">Sign Up Form</h2>
                <form @submit.prevent="formSubmitted" class="px-20"> 
                    <div v-for="error in errors" :key="error"> <span>{{ error }}</span> </div>
            
                            <div class="pt-12 pb-8 ">
                                <div class="flex "> 
                                    <label for="name" class="block text-gray-700 text-sm font-bold mb-2 mr-2">FirstName</label>
                                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" class="w-2 h-2 mt-2 fill-red-500"><path d="M478.21 334.093L336 256l142.21-78.093c11.795-6.477 15.961-21.384 9.232-33.037l-19.48-33.741c-6.728-11.653-21.72-15.499-33.227-8.523L296 186.718l3.475-162.204C299.763 11.061 288.937 0 275.48 0h-38.96c-13.456 0-24.283 11.061-23.994 24.514L216 186.718 77.265 102.607c-11.506-6.976-26.499-3.13-33.227 8.523l-19.48 33.741c-6.728 11.653-2.562 26.56 9.233 33.037L176 256 33.79 334.093c-11.795 6.477-15.961 21.384-9.232 33.037l19.48 33.741c6.728 11.653 21.721 15.499 33.227 8.523L216 325.282l-3.475 162.204C212.237 500.939 223.064 512 236.52 512h38.961c13.456 0 24.283-11.061 23.995-24.514L296 325.282l138.735 84.111c11.506 6.976 26.499 3.13 33.227-8.523l19.48-33.741c6.728-11.653 2.563-26.559-9.232-33.036z"/></svg>

                                </div> 

                                <input id="name" type="text" v-model="firstname" class="drop-shadow-2xl appearance-none border rounded w-3/4 py-2 px-3">

                               
                            </div>
                            <div class=" pb-8 ">
                                <div class="flex "> 
                                    <label for="name" class="block text-gray-700 text-sm font-bold mb-2 mr-2">LastName</label>
                                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" class="w-2 h-2 mt-2 fill-red-500"><path d="M478.21 334.093L336 256l142.21-78.093c11.795-6.477 15.961-21.384 9.232-33.037l-19.48-33.741c-6.728-11.653-21.72-15.499-33.227-8.523L296 186.718l3.475-162.204C299.763 11.061 288.937 0 275.48 0h-38.96c-13.456 0-24.283 11.061-23.994 24.514L216 186.718 77.265 102.607c-11.506-6.976-26.499-3.13-33.227 8.523l-19.48 33.741c-6.728 11.653-2.562 26.56 9.233 33.037L176 256 33.79 334.093c-11.795 6.477-15.961 21.384-9.232 33.037l19.48 33.741c6.728 11.653 21.721 15.499 33.227 8.523L216 325.282l-3.475 162.204C212.237 500.939 223.064 512 236.52 512h38.961c13.456 0 24.283-11.061 23.995-24.514L296 325.282l138.735 84.111c11.506 6.976 26.499 3.13 33.227-8.523l19.48-33.741c6.728-11.653 2.563-26.559-9.232-33.036z"/></svg>

                                </div> 

                                <input id="name" type="text" v-model="lastname" class="drop-shadow-2xl appearance-none border rounded w-3/4 py-2 px-3">

                               
                            </div>
                            <div class=" pb-8 ">
                                <div class="flex "> 
                                    <label for="name" class="block text-gray-700 text-sm font-bold mb-2 mr-2">Email</label>
                                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" class="w-2 h-2 mt-2 fill-red-500"><path d="M478.21 334.093L336 256l142.21-78.093c11.795-6.477 15.961-21.384 9.232-33.037l-19.48-33.741c-6.728-11.653-21.72-15.499-33.227-8.523L296 186.718l3.475-162.204C299.763 11.061 288.937 0 275.48 0h-38.96c-13.456 0-24.283 11.061-23.994 24.514L216 186.718 77.265 102.607c-11.506-6.976-26.499-3.13-33.227 8.523l-19.48 33.741c-6.728 11.653-2.562 26.56 9.233 33.037L176 256 33.79 334.093c-11.795 6.477-15.961 21.384-9.232 33.037l19.48 33.741c6.728 11.653 21.721 15.499 33.227 8.523L216 325.282l-3.475 162.204C212.237 500.939 223.064 512 236.52 512h38.961c13.456 0 24.283-11.061 23.995-24.514L296 325.282l138.735 84.111c11.506 6.976 26.499 3.13 33.227-8.523l19.48-33.741c6.728-11.653 2.563-26.559-9.232-33.036z"/></svg>

                                </div> 

                                <input id="name" type="email" v-model="email" class="drop-shadow-2xl appearance-none border rounded w-3/4 py-2 px-3">

                               
                            </div>
                            <div class=" pb-8 ">
                                <div class="flex "> 
                                    <label for="name" class="block text-gray-700 text-sm font-bold mb-2 mr-2">Password</label>
                                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" class="w-2 h-2 mt-2 fill-red-500"><path d="M478.21 334.093L336 256l142.21-78.093c11.795-6.477 15.961-21.384 9.232-33.037l-19.48-33.741c-6.728-11.653-21.72-15.499-33.227-8.523L296 186.718l3.475-162.204C299.763 11.061 288.937 0 275.48 0h-38.96c-13.456 0-24.283 11.061-23.994 24.514L216 186.718 77.265 102.607c-11.506-6.976-26.499-3.13-33.227 8.523l-19.48 33.741c-6.728 11.653-2.562 26.56 9.233 33.037L176 256 33.79 334.093c-11.795 6.477-15.961 21.384-9.232 33.037l19.48 33.741c6.728 11.653 21.721 15.499 33.227 8.523L216 325.282l-3.475 162.204C212.237 500.939 223.064 512 236.52 512h38.961c13.456 0 24.283-11.061 23.995-24.514L296 325.282l138.735 84.111c11.506 6.976 26.499 3.13 33.227-8.523l19.48-33.741c6.728-11.653 2.563-26.559-9.232-33.036z"/></svg>

                                </div> 

                                <input id="name" type="password" v-model="password" class="drop-shadow-2xl appearance-none border rounded w-3/4 py-2 px-3">

                               
                            </div>
                            
                          
                            <button type="submit" value="Submit" class="bg-pink-600 text-white font-semibold py-3 px-12 rounded drop-shadow-2xl " >Submit</button>
        
                        </form>
            </div>
    
            <div class="w-full shadow-md "> 
                <img src="../assets/paint.jpg" class="w-full h-[720px] object-cover object-top">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ValidateForm',
    props: {
        msg: String
    },

    data(){
        return{
            firstname: null,
            lastname: null,
            email: null,
            password:null,
            errors: [],

        }
    },

    methods: {
        formSubmitted(){
            this.errors =[];
            if(!this.firstname){
                this.errors.push("Firstname is required, please fill it.");
                this.firstname = ''

            }
            if(!this.lastname){
                this.errors.push("Lastname is required, please fill it.");

            }
            if(!this.email){
                this.errors.push("Email is required, please fill it.");


            }
            if(!this.password){
                this.errors.push("Password is required, please fill it.");

            }
        

        },

    }


}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
