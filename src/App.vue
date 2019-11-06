<template>
  <div id="app">{{ hello }}</div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      hello: "preset value"
    };
  },
  async created() {
    let { helloworld } = await import("./helloworld.js");
    this.hello = helloworld.sayHello();
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
