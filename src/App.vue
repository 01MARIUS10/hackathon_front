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
      <Navbar />
  </header>
<div class="view">
  <RouterView />
</div>
</template>

<style >
  header,#nav{
    height: 60px;
  }
  view{
    margin-top: 60px;
  }
</style>

