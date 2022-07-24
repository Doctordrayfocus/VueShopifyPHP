<template>
  <div
    class="w-full py-5 flex flex-col space-y-3 justify-center items-center bg-blue-100 mt-6"
  >
    <h1>This is the sample index page</h1>
    <router-view></router-view>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { useMeta } from "vue-meta";

export default defineComponent({
  name: "SampleIndexPage",
  layout: "Sample",
  setup() {
    useMeta({
      title: "Sample Index Page",
    });
    return {};
  },
});
</script>
