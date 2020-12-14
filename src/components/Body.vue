<template>
  <div id="body">
    <span class="no-items-message">No Items</span>
    <all-items v-bind:adr="adr"></all-items>
  </div>
</template>

<script>
import AllItems from "./AllItems"
export default {
  name: "Body",
  components: {
    "all-items": AllItems
  },
  props: ["adr"]
 
};
</script>

<style>
</style>
