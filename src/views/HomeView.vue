<script lang="ts">
import { defineComponent } from 'vue';

  export default defineComponent({
    name: 'App',
    components: {},
    data() {
      return {
        name: 'Link',
        age: 34 as number | string
      }
    },
    methods: {
      changeName(name: string){
        this.name = name;
      }
    }
  })
</script>

<template>
  <main class="center">
    <h2>Hello {{name}}</h2><h2>Welcome to Dev Jobs</h2>
    <button @click="changeName('Raymond')" class="button">Change Name</button>
  </main>
</template>


<style scoped>
  @import "@/assets/styles/buttons.css";
</style>
