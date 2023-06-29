<script lang="ts">
import Hello from '../components/molecules/testComponent.vue'
import Navbar from '../components/shared/navbar.vue'
import caroussel from '../components/molecules/carousel.vue'
import landingPage from '../components/molecules/landingPage.vue'
import { defineComponent } from 'vue';

export default defineComponent({
  components:{Hello,Navbar,caroussel,landingPage},
  methods:{

  }
})
</script>

<template>
  <main id="home">
    <landingPage/>
  </main>
</template>
