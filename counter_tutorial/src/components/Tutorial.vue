<template>
  <div class="counter_container">
    <div class="vue_header">
      <h1>Vue Counter Project</h1>
    </div>
    <div class="vue_counter">
      {{count}}
    </div>
    <div class="vue_buttons">
      <button class="increment" @click="increment">Increment</button>
      <button class="decrement" @click="decrement">Decrement</button>
      <button class="reset" @click="reset">Reset</button>
    </div>
  </div>
</template>
<script>
export default {
  name:"Tutorial",
  data() {
    return {
      count:0,
    }
  },
  methods: {
    increment() {
      this.count++
    },
    decrement() {
      this.count--
    },
    reset()  {
      this.count = 0
    }
  }
}
</script>
<style scoped>
.counter_container {
  height: 100vh;
  position: relative;
  width:100%;
  overflow: hidden;
}
.vue_header {
  text-align: center;
  margin-top: 15%;
}
.vue_counter {
  font-size: 80px;
}
.increment {
  font-size: 15px;
  padding: 10px 20px;
    border-radius: 5px;
  outline: none;
  background: #039603;
  color: #fff;
  border: none;
}
.decrement {
  font-size: 15px;
  padding: 10px 20px;
  background: #ff0000;
  color: #fff;
  margin: 10px;
  border-radius: 5px;
  outline: none;
  border: none;
}
.reset {
  font-size: 15px;
  padding: 10px 20px;
    border-radius: 5px;
  outline: none;
  border: none;
}
.vue_counter,.vue_buttons {
  text-align: center;
  margin-top: 5%;
}
@media(max-width:700px) {
  .counter_container {
    overflow: hidden;
    position: relative;
  }
  .vue_header {
    text-align: center;
  }
  .vue_header h1 {
    font-size: 20px;
  }
  .vue_counter {
    font-size: 30px;
    text-align: center;
  }
  .vue_buttons {
     text-align: center;
  }
  .increment,.decrement,.reset {
    font-size: 10px;
    padding: 5px 10px;
  }
}
</style>
