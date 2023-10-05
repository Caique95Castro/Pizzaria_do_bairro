<template>
    <div class="contato">
      
      <ContatoWorld />
    </div>
  </template>
  
  <script>
  // @ is an alias to /src
  import ContatoWorld from '@/components/ContatoWorld.vue'
  
  export default {
    name: 'HomeView',
    components: {
        ContatoWorld
    }
  }
  </script>
  