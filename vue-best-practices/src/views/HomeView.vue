<template>
  <div class="home">
    {{ value }}
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";
// import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src

// Using Composition API instead of Options API.
export default defineComponent({
  name: "HomeView",
  components: {},
  props: {},
  setup: (props) => {
    const value = ref<string>("test is here");

    // const isAdmin = computed(() => store.getters.isAdmin);

    // watch(
    //   () => props.letter,
    //   async () => {
    //     await getPeople();
    //   }
    // );

    return {
      value,
    };
  },
});
</script>
