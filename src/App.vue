<template>
  <div class="app">
    <p>Hello, {{ name }}!</p>
    <button @click="changeName('Zelda')">Change Name</button>
    <p>Your age is: {{ age }}!</p>
    <button @click="changeAge(26)">Change Age</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'App',
  components: {

  },
  data() {
    return {
      name: 'Link',
      age: 25
    };
  },
  methods: {
    changeName(name: string) {
      this.name = name;
    },
    changeAge(age: number) {
      this.age = age;
    }
  }
});
</script>

<style>

</style>
