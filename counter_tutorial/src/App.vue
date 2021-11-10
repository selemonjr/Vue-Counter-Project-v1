<template>
<Tutorial/>
</template>
<script>
import Tutorial from "./components/Tutorial.vue";
export default {
  name:"App",
  components: {
    Tutorial,
  },
}
</script>
<style>
* {
  margin:0;
  padding:0;
  box-sizing:border-box;
}
body {
  height: 100vh;
  width: 100%;
  position: relative;
  font-family: sans-serif;
  display: grid;
  place-items: center;
}
</style>
