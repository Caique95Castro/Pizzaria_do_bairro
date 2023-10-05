<template>
    <div class="cardapio">
      
      <CardapioWorld />
    </div>
  </template>
  
  <script>
  // @ is an alias to /src
  import CardapioWorld from '@/components/CardapioWorld.vue'
  
  export default {
    name: 'HomeView',
    components: {
        CardapioWorld
    }
  }
  </script>
  