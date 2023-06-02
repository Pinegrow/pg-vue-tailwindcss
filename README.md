# Vue Designer Tailwind CSS - Quick start template

This is a starter template that pre-includes the [Pinegrow Vite Plugin](https://www.npmjs.com/package/@pinegrow/vite-plugin), [Pinegrow Tailwind CSS Plugin](https://www.npmjs.com/package/@pinegrow/tailwindcss-plugin) and other goodies for Vue Designer.

## Vue Designer

A desktop drag-and-drop editor for Vue apps supporting Mac, Windows and Linux by [Pinegrow](https://pinegrow.com/).

It let's you visually design 🎨 your Vue single file components and boosts your productivity and your creativity while building your component-based Vue apps.

It smartly integrates with your ⚡️ [Vite](https://vitejs.dev/) based CLI, and provides an amazing deverloper experience with it's powerful visual controls and features.

Clean code 😃, No lock-in - Pinegrow Vue Designer is an open-tool ❤️

## Try it now!

### 1. Clone to local

[Create a repo from this template on GitHub](https://github.com/pinegrow/pg-vue-tailwindcss/generate).

(or)

If you prefer to do it manually with the cleaner git history

```bash
npx giget@latest gh:pinegrow/pg-vue-tailwindcss my-vue-tailwindcss-app #project-name
cd my-vue-tailwindcss-app
npm install #or use pnpm
```

## 2. Open in Vue Designer

Open your project in Vue Designer, and follow the instructions displayed in the Config Panel (that should pop-out automatically). Config Panel ⚙️ displays the key packages and the various links to their individual ecosystem and community.

## Usage

### Start your development server

```bash
npm run dev
```

### Preview

```bash
npm run now # build & preview
```

### Build

```bash
npm run build # SPA
```

And you will see the generated file in `dist` that's ready to be served.

### Deploy on Netlify

Go to [Netlify](https://app.netlify.com/start) and select your clone, `OK` along the way, and your app will be live in a minute.

Check out the [deployment documentation](https://vitejs.dev/guide/static-deploy.html#netlify) for more information.

## Pre-packed

### Meta Framework (Vue-based)

- [Vite](https://vitejs.dev/) - Vite-powered Vue SPA
  - 👉 Follow the amazing Vue [docs](https://vuejs.org/guide/introduction.html)

### UI Frameworks

- [Tailwind CSS](https://tailwindcss.com/docs/guides/vite#vue) - The amazing utility-first CSS framework.

### Filed-based CMS (markdown)

- [Vite-plugin-vue-markdown](https://github.com/mdit-vue/vite-plugin-vue-markdown) - file-based CMS for powered by Markdown & Vue components. Note: This page is a markdown file 🗒.

### Icons

- [UnoCSS Preset Icons](https://github.com/unocss/unocss/tree/main/packages/preset-icons/) - use over 100,000 open-source [Iconify](https://iconify.design/) icons. Uses the **unocss** format for icon names, for eg, `i-mdi-home`.

### Modules/Plugins

- [VueUse](https://vueuse.org/) - collection of essential Vue composition utilities.
- [Pinegrow Vite Plugin](https://www.npmjs.com/package/@pinegrow/vite-plugin) - enables you to live-design your Vue single-file-components visually in Vue Designer.
- [Pinegrow Tailwind CSS Plugin](https://www.npmjs.com/package/@pinegrow/tailwindcss-plugin) - via Design Panel, enables visual controls customization (automatic) and theme customization (optional).

### Devtools

- [Vue Devtools](https://devtools.vuejs.org/guide/installation.html#standalone) - Official devtools that can be used as a standalone app alongside Vue Designer. It's conditionally configured in `main.ts` (only during development).
  - **ACTION REQUIRED**: Currently deactivated. In `main.ts`, uncomment the top devtools related snippet to activate.
- [Vite Devtools](https://github.com/webfansplz/vite-plugin-vue-devtools) - A Vite plugin for Vue that enhances your DX (developer experience) with an amazing set of in-app features. This is an in-app alternative to browser-based/standalone Vue Devtools.

### VS Code Extensions

- [VS Code Extensions](./.vscode/extensions.json)
  - [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) - Vue 3 `<script setup>` IDE support
  - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
  - [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

### Coding Style

- Use Composition API with [`<script setup>` SFC syntax](https://vuejs.org/guide/scaling-up/sfc.html)
- [ESLint](https://eslint.org) with [eslint-plugin-vue](https://vuejs.org/guide/scaling-up/tooling.html#linting) - official set of linting rules.
- [Prettier](https://prettier.io) with [@vue/eslint-config-prettier](https://vuejs.org/guide/scaling-up/tooling.html#formatting) - format without conflicting with eslint rules.

### Typescript

Allows JS & strict mode is turned off. Update `tsconfig.ts` as required.

```json
{
  "compilerOptions": {
    // ...
    "strict": false,
    "allowJs": true
  }
}
```

## Community

- [Pinegrow Vue Designer](https://forum.pinegrow.com/vue-designer)
