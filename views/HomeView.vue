<script lang="ts">
import Hello from '../components/testComponent.vue'
import { defineComponent } from 'vue';
export default defineComponent({
  name:'homeView',
  components:{Hello}
})
</script>

<template>
  <main>
    <Hello />
  </main>
</template>
