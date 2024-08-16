<script lang="ts">
import { defineComponent } from 'vue';

  export default defineComponent({
    name: 'App',
    components: {},
    data() {
      return {
        name: 'Link'
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
  <main>
    <h2>Hello {{name}}</h2><h2>Welcome to Dev Jobs</h2>
    <button @click="changeName('Raymond')">Change Name</button>
  </main>
</template>
