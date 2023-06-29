<script lang="ts">
import Hello from '../components/molecules/testComponent.vue'
import Navbar from '../components/shared/navbar.vue'
import caroussel from '../components/molecules/carousel.vue'
import { defineComponent } from 'vue';

export default defineComponent({
  components:{Hello,Navbar,caroussel},
  methods:{

  }
})
</script>

<template>
  <main id="home">
    <Hello />
    <caroussel />
  </main>
</template>
