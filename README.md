# diwa401 README / LEEME

## Instructions to run
To run the project as it's uploaded, you need to run the next commands:
```bash
npm i
npm start
```
## From initial code to tailwindcss solution

To get from the initial code to the current code, you need to execute the next commands:

```bash
npm i vite tailwindcss postcss

npx tailwindcss init
```

Create a file name vite.config.js with the next contents:

```
import { defineConfig } from 'vite'

// https://vitejs.dev/config/
export default defineConfig({
  plugins: [],
})

```
Set up the tailwind config as this one:
```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./**/*.{html,js}"
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}

```
And in package.json setup the section scripts as this one:
```
  "scripts": {
    "start": "vite",
    "build": "vite build"
  }
```

Add the tailwind directives in main.css:
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

Run this command and open the URL in the browser:
```bash
npm start
```
## Context
*Unidad:* UD03. Frameworks CSS

*Módulo:* Diseño de Interfaces WEB

*Ciclo Formativo:* Desarrollo de Aplicaciones WEB

### Author / Autor
Aarón Martín Bermejo