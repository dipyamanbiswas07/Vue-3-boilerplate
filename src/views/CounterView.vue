<script setup lang="ts">
import { useCounterStore } from '@/stores/counter'

const counter = useCounterStore()
</script>

<template>
  <div class="counter">
    <h1>Counter Example</h1>
    <p>This demonstrates Pinia state management</p>

    <div class="counter-display">
      <h2>{{ counter.count }}</h2>
    </div>

    <div class="counter-controls">
      <button @click="counter.decrement">-</button>
      <button @click="counter.increment">+</button>
    </div>

    <p>Double count: {{ counter.doubleCount }}</p>
  </div>
</template>

<style scoped>
.counter {
  text-align: center;
  padding: 2rem;
}

.counter-display {
  margin: 2rem 0;
}

.counter-display h2 {
  font-size: 4rem;
  color: var(--color-text);
  margin: 0;
}

.counter-controls {
  display: flex;
  gap: 1rem;
  justify-content: center;
  margin: 2rem 0;
}

.counter-controls button {
  padding: 1rem 2rem;
  font-size: 1.5rem;
  background-color: var(--color-background-soft);
  border: 2px solid var(--color-border);
  border-radius: 8px;
  cursor: pointer;
  transition: all 0.2s;
}

.counter-controls button:hover {
  background-color: var(--color-background-mute);
  border-color: var(--color-border-hover);
}

.counter-controls button:active {
  transform: scale(0.98);
}
</style>
