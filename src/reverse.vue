<template>
  <div>
    <h1>{{ msg }}</h1>
    <button @click="click">翻转</button>
  </div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      msg: "HOLLE,VUE!",
    };
  },
  methods: {
    click() {
      this.msg = this.msg.split("").reverse().join("");
    },
  },
};
</script>

<style></style>
