# Vue 3 Boilerplate

A modern Vue 3 boilerplate project with TypeScript, Vite, Vue Router, and Pinia.

## Features

- ⚡️ **Vue 3** - The latest version of Vue.js with Composition API
- 🔥 **TypeScript** - Type safety and better developer experience
- 🚀 **Vite** - Fast build tool and development server
- 🛣️ **Vue Router** - Official router for Vue.js
- 🗄️ **Pinia** - Intuitive state management for Vue
- 🧪 **Vitest** - Fast unit testing framework
- 📏 **ESLint** - Code linting and formatting
- 💅 **Prettier** - Code formatting
- 🎨 **Modern CSS** - CSS variables and responsive design

## Project Structure

```
src/
├── assets/          # Static assets (CSS, images, etc.)
├── components/      # Reusable Vue components
│   └── icons/       # Icon components
├── router/          # Vue Router configuration
├── stores/          # Pinia stores
├── views/           # Page components
├── App.vue          # Root component
└── main.ts          # Application entry point
```

## Getting Started

### Prerequisites

- Node.js (version 16 or higher)
- npm or yarn

### Installation

1. Clone the repository or use this template
2. Install dependencies:

```bash
npm install
```

### Development

Start the development server:

```bash
npm run dev
```

The application will be available at `http://localhost:3000`

### Build

Build for production:

```bash
npm run build
```

### Preview

Preview the production build:

```bash
npm run preview
```

### Testing

Run unit tests:

```bash
npm run test
```

### Linting

Run ESLint:

```bash
npm run lint
```

Format code with Prettier:

```bash
npm run format
```

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run test` - Run unit tests
- `npm run lint` - Run ESLint
- `npm run format` - Format code with Prettier

## Usage

### Adding Components

Create new components in the `src/components/` directory. Use the composition API with `<script setup>`:

```vue
<script setup lang="ts">
import { ref } from 'vue'

const count = ref(0)

const increment = () => {
  count.value++
}
</script>

<template>
  <button @click="increment">Count: {{ count }}</button>
</template>
```

### State Management

Use Pinia stores for state management. Create stores in `src/stores/`:

```typescript
import { ref, computed } from 'vue'
import { defineStore } from 'pinia'

export const useCounterStore = defineStore('counter', () => {
  const count = ref(0)
  const doubleCount = computed(() => count.value * 2)
  
  function increment() {
    count.value++
  }

  return { count, doubleCount, increment }
})
```

### Routing

Add new routes in `src/router/index.ts`:

```typescript
{
  path: '/new-page',
  name: 'NewPage',
  component: () => import('../views/NewPageView.vue')
}
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Run tests and linting
5. Submit a pull request

## License

MIT License - see the [LICENSE](LICENSE) file for details.
