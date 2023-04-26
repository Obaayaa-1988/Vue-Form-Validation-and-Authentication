<template>
    <div class="w-[90%] mx-auto py-20"> 
        <div class="flex"> 
            <div class="bg-white w-[90%] h-[720px] mx-auto shadow-md rounded-l-lg">
                <h2 class="bg-pink-600 text-2xl py-4 text-white text-center rounded-l-lg font-bold">Sign Up Form</h2>
                <!-- <div class="text-center"> 
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-20 h-20 font-extrabold">
      <path stroke-linecap="round" stroke-linejoin="round" d="M17.982 18.725A7.488 7.488 0 0012 15.75a7.488 7.488 0 00-5.982 2.975m11.963 0a9 9 0 10-11.963 0m11.963 0A8.966 8.966 0 0112 21a8.966 8.966 0 01-5.982-2.275M15 9.75a3 3 0 11-6 0 3 3 0 016 0z" />
    </svg>

                </div> -->
                <form @submit.prevent="formSubmitted" class="px-20"> 
            
                            <p class="pt-12 pb-8"> 
                                <label for="name" class="block text-gray-700 text-sm font-bold mb-2">FirstName:</label>
                                <input id="name" type="text" v-model="firstname" class="drop-shadow-2xl appearance-none border rounded w-3/4 py-2 px-3">
                            </p>
                            <p> 
                                <label for="name" class="block text-gray-700 text-sm font-bold mb-2">LastName:</label>
                                <input id="name" type="text" v-model="lastname" class="drop-shadow-2xl appearance-none border rounded w-3/4 py-2 px-3">
                            </p>
                            <p class="py-8"> 
                                <label for="name" class="block text-gray-700 text-sm font-bold mb-2">Email:</label>
                                <input id="name" type="email" v-model="email" class="drop-shadow-2xl appearance-none border rounded w-3/4 py-2 px-3">
                            </p>
                            <p class="pb-8"> 
                                <label for="name" class="block text-gray-700 text-sm font-bold mb-2">Password:</label>
                                <input id="name" type="password" v-model="password" class="drop-shadow-2xl appearance-none border rounded w-3/4 py-2 px-3">
                            </p>
                            <!-- <p> 
                                <label for="reviews">Comment:</label>
                             <textarea id="review" v-model="review"></textarea>
            
                            </p>
             -->
                            <button type="submit" value="Submit" class="bg-pink-600 text-white font-semibold py-3 px-12 rounded drop-shadow-2xl " >Submit</button>
        
                        </form>
            </div>
    
            <div class="w-full shadow-md "> 
                <img src="../assets/paint.jpg" class="w-[90%] h-[720px] object-cover object-top">
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
            
           

        },

    }


}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
