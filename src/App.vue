<template>
  <div id="app">
    <Mouse :renderProp="__render"/>
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
    __render({ x, y }) {
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