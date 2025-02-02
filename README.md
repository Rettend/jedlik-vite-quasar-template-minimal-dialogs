# `Vue 3.x + Quasar 2.x template with Vite`

# Take Over Mode

To get Vue SFCs and TypeScript working together, Volar creates a separate TS language service instance patched with Vue-specific support, and uses it in Vue SFCs. At the same time, plain TS files are still handled by VSCode's built-in TS language service, which is why we need TypeScript Vue Plugin to support Vue SFC imports in TS files. This default setup works, but for each project we are running two TS language service instances: one from Volar, one from VSCode's built-in service. This is a bit inefficient and can lead to performance issues in large projects.

Volar provides a feature called "Takeover Mode" to improve performance. In takeover mode, Volar provides support for both Vue and TS files using a single TS language service instance.

## Enable Take Over Mode

1. Disable built-in TypeScript extension:

- Run Extensions: Show Built-in Extensions command
- Find "TypeScript and JavaScript Language Features", right click and select: Disable (Workspace)

2. Reload VSCode

# Debug your application

- Start build process with Ctrl-Shift-B or "npm run dev" command
- Close the borwser if it appears
- Open the default browser in debug mode with F5 key
- Open the page where you want to debug the code
- Set some breakpoints before lines in the page's TS code
- In the browser cause the process to reach the breakpoint(S)
- Examine the variables, continue the execution step by step (F10, F11, for next breakpont: F5)

# Used technologies

## Node.js

As an asynchronous event-driven JavaScript runtime, [Node.js](https://nodejs.org/en/) is designed to build scalable network applications.

## Vue.js

[Vue.js](https://vuejs.org/) is an approachable, performant and versatile framework for building web user interfaces.

## Vue.js 3 Composition API

[Composition API](https://vuejs.org/api/composition-api-setup.html) is a set of APIs that allows us to author Vue components using imported functions instead of declaring options.

## Vue.js 3 SFC and "script setup"

["script setup"](https://vuejs.org/api/sfc-script-setup.html) is a compile-time syntactic sugar for using Composition API inside Single File Components (SFCs). It is the recommended syntax if you are using both SFCs and Composition API.

## Vue Router

["Vue Router"](https://router.vuejs.org/) is the official router for Vue.js. It deeply integrates with Vue.js core to make building Single Page Applications with Vue.js a breeze.

## VueUse

["VueUse"](https://vueuse.org/) is a collection of utility functions based on Composition API. We assume you are already familiar with the basic ideas of Composition API before you continue.

## TypeScript

[TypeScript](https://www.typescriptlang.org/) is a strongly typed programming language that builds on JavaScript, giving you better tooling at any scale.

## Quasar

With [Quasar](https://quasar.dev/) you can build effortlessly build high-performance & high-quality Vue.js 3 user interfaces in record time. ["Awesome Quasar"](https://github.com/quasarframework/quasar-awesome)

## Axios

[Axios](https://axios-http.com/) is a simple promise based HTTP client for the browser and node.js. Axios provides a simple to use library in a small package with a very extensible interface. [GitHub](https://github.com/axios/axios)

## Pinia

[Pinia](https://pinia.vuejs.org/) is a store library for Vue, it allows you to share a state across components/pages.

## Pinia Pugin Persist

[Persist](https://github.com/Seb-L/pinia-plugin-persist) VueJs Pinia state data in sessionStorage or other storages, heavilly influenced by vuex-persistedstate.

## Vite

[Vite](https://vitejs.dev/) is a build tool that aims to provide a faster and leaner development experience for modern web projects. It consists a dev server that provides rich feature enhancements over native ES modules, for example extremely fast Hot Module Replacement (HMR).

## vue-i18n

[vue-i18n](https://github.com/intlify/vue-i18n-next/tree/master/packages/vue-i18n#readme) Internationalization plugin for Vue.js

## ESlint

[ESLint](https://eslint.org/) statically analyzes your code to quickly find problems. Many problems ESLint finds can be automatically fixed. Preprocess code, use custom parsers, and write your own rules that work alongside ESLint's built-in rules. You can customize ESLint to work exactly the way you need it for your project.

## Prettier

[Prettier](https://prettier.io/) an opinionated code formatter. Supports many languages, integrates with most editors.

## Vitest for unit and components tests

Since the official setup created by create-vue is based on Vite, we recommend using a unit testing framework that can leverage the same configuration and transform pipeline directly from Vite. ["Vitest"](https://vuejs.org/guide/scaling-up/testing.html#unit-testing) is a unit testing framework designed specifically for this purpose, created and maintained by Vue / Vite team members. It integrates with Vite-based projects with minimal effort, and is blazing fast.

## Cypress

Until now, end-to-end testing wasn’t easy. It was the part developers hated.
Not anymore. ["Cypress"](https://www.cypress.io/) makes setting up, writing, running and debugging tests easy.
