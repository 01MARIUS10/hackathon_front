<script lang="ts">
import { RouterView } from 'vue-router'
import { defineComponent } from 'vue';
import Navbar from './components/shared/navbar.vue'

export default defineComponent({
  components:{Navbar},

})
</script>

<template>
  <header>
    <div class="">
      <Navbar />
    </div>
  </header>

  <RouterView />
</template>

<style scoped>

</style>

