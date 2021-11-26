<template>
  <div class="app">
    <!-- <p>Hello, {{ name }}!</p>
    <button @click="changeName('Zelda')">Change Name</button>
    <p>Your age is: {{ age }}!</p>
    <button @click="changeAge(26)">Change Age</button> -->

    <p>{{ jobs[0].title }}</p>
  </div>
</template>

<script lang="ts">
import { defineComponent, reactive, ref, toRefs } from "vue";
import Job from "./types/job";

export default defineComponent({
  name: "App",
  components: {},
  setup() {
    //   const state = reactive({
    //     name: "Link",
    //     age: 0,
    //   });

    //   state.name = "Tyler";

    //   return { ...toRefs(state) };

    // const name = ref("Link");
    // const age = ref(0);

    // return { name, age };

    const jobs = ref<Job[]>([
      { title: "Link", location: "Hyrule", salary: 70000, id: "1" },
      { title: "Zelda", location: "Hyrule", salary: 70000, id: "1" }
      ]);

      return 
  },
  // methods: {
  //   changeName(name: string) {
  //     this.name = name;
  //   },
  //   changeAge(age: number) {
  //     this.age = age;
  //   },
  // },

});
</script>

<style></style>
