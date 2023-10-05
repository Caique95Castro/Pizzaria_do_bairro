<template>
  <div class="about">
    
    <AboutWorld />
  </div>
</template>

<script>
// @ is an alias to /src
import AboutWorld from '@/components/AboutWorld.vue'

export default {
  name: 'AboutView',
  components: {
    AboutWorld
  }
}
</script>
