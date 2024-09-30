<template>
  <div>
    <h1>Simple Counter</h1>
    <p>Count: {{ count }}</p>
    <button @click="increase">Increase</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Counter',
  data() {
    return {
      count: 0
    }
  },
  methods: {
    increase(): void {
      this.count += 8
    }
  }
})
</script>

<style scoped>
div {
  text-align: center;
}

button {
  padding: 10px 20px;
  font-size: 16px;
  background-color: orangered;
  color: white;
  border: none;
}
</style>
