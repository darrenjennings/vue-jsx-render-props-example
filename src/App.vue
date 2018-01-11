<template>
  <div id="app">
    <Mouse :render="renderPosition" />
  </div>
</template>

<script>
import Mouse from "./components/Mouse.js";

export default {
  name: "app",
  components: {
    Mouse
  },
  methods: {
    renderPosition({ x, y }) {
      return (
        <h1>
          The mouse position is ({x}, {y})
        </h1>
      );
    }
  }
};
</script>
<style>
* {
  margin: 0;
  height: 100%;
  width: 100%;
}
</style>