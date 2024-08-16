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
    changeName(name: string) {
      this.name = name;
    }
  }
})
</script>

<template>
  <!-- <main class="center"> -->
    <div class="flex flex-col w-screen h-screen bg-white items-center justify-center">
    <div class="flex flex-col relative h-full w-full">
      <main class="flex flex-col h-full w-full bg-gray-10">
        <div class="flex flex-row h-full">
          <div class="flex flex-col flex-grow rounded p-2">
            <div class="relative overflow-y-auto w-full flex-grow" style="border-radius:12px">
              <h2>Hello {{ name }}</h2>
              <h2>Welcome to Dev Jobs</h2>
              <RouterView />

              <button @click="changeName('Raymond')" class="button">Change Name</button>
            </div>
          </div>
        </div>
      </main>
    </div>
  </div>
  <!-- </main> -->
</template>


<style scoped>
@import "@/assets/styles/buttons.css";
</style>
