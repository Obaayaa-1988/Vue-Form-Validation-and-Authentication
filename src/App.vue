<template>
  <div class=" bg-gradient-to-r from-cyan-500 to-orange-500 h-screen w-full"> 
    <ValidateForm />
   
  </div>
</template>

<script>
 import ValidateForm from './components/ValidateForm.vue'

export default {
  name: 'App',
  components: {
    ValidateForm
  }
}
</script>

<style>
</style>
