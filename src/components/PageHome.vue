<template>
  <div class="col-full">
    <h1>welcome to the forum</h1>
    <ThreadList :threads="threads" />
  </div>
</template>

<script>
import sourceData from "@/data.json";
import ThreadList from "./ThreadList.vue";
export default {
  data() {
    return {
      threads: sourceData.threads,
    };
  },
  components: {
    ThreadList,
  },
};
</script>

<style></style>
