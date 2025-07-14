<template>
  <div class="about">
    <h1>This is an about page</h1>
    <p>
      This is a Vue 3 boilerplate project built with TypeScript, Vite, Vue Router, and Pinia. It
      includes modern development tools and best practices for Vue.js development.
    </p>
    <h2>Features</h2>
    <ul>
      <li>Vue 3 with Composition API</li>
      <li>TypeScript support</li>
      <li>Vue Router for navigation</li>
      <li>Pinia for state management</li>
      <li>Vite for fast development</li>
      <li>ESLint and Prettier for code quality</li>
      <li>Vitest for testing</li>
    </ul>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 2rem;
  }
}
</style>
