<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

# Vue 3 Boilerplate Project Instructions

This is a Vue 3 project built with TypeScript, Vite, Vue Router, and Pinia. Please follow these guidelines when generating code:

## Framework and Tools
- Use Vue 3 with Composition API and `<script setup>` syntax
- TypeScript should be used for all logic
- Use Pinia for state management with the composition API style
- Use Vue Router for navigation
- Vite is used as the build tool

## Code Style
- Use single quotes for strings
- No semicolons
- 2 spaces for indentation
- Use trailing commas sparingly
- Prefer arrow functions where appropriate

## Component Structure
- Use `<script setup lang="ts">` for all Vue components
- Place imports at the top of the script section
- Use proper TypeScript typing for props and emits
- Use CSS modules or scoped styles

## State Management
- Use Pinia stores with the composition API pattern
- Export stores using the `useStoreName` convention
- Use `ref` and `computed` from Vue for reactive state

## Testing
- Use Vitest for unit testing
- Use Vue Test Utils for component testing
- Place tests in `__tests__` directories or use `.test.ts` suffixes

## Best Practices
- Use proper semantic HTML
- Implement proper accessibility features
- Use CSS custom properties for theming
- Follow Vue 3 best practices and patterns
- Use modern JavaScript/TypeScript features
