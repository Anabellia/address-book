<template>
  <div id="footer">
    <input type="text" placeholder="Input your name in here.." v-model="content.name" />
    <input type="text" placeholder="Input your number in here.." v-model="content.number" />
    <button v-on:click="onClick" >Add</button>
  </div>
</template>

<script>

export default {
  name: "Footer",
  data: function () {
    return {
      content: {
         name: "", 
         number: "" 
      }
    };
  },
  methods: {
    onClick: function() {
      this.$emit("item-add", this.content);
    }
  }
};
</script>

<style>
</style>
