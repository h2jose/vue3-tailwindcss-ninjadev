# vue3-tailwindcss

This template should help get you started developing with Vue 3 in Vite.

## 1  Introduction

```sh
npm init vue@latest
```

## 2 Tailwind setup

```sh
npm install -D tailwindcss postcss autoprefixer
```

```sh
 npx tailwindcss init -p
```

Tailwind.config.js

```sh
module.exports = {
  content: ["./index.html", "./src/**/*.{vue,js,ts,jsx,tsx}"],
  theme: {
    extend: {
      colors: {
        "weather-primary": "#00668A",
        "weather-secondary": "#004E71",
      },
    },
    fontFamily: {
      Roboto: ["Roboto, sans-serif"],
    },
    container: {
      padding: "2rem",
      center: true,
    },
    screens: {
      sm: "640px",
      md: "768px",
    },
  },
  plugins: [],
};
```

assets/tailwind.css

```sh
@tailwind base;
@tailwind components;
@tailwind utilities;
```

main.js

```sh
import "./assets/tailwind.css"
```

## 3 Navbar

- cdnjs.com Font-awesome library
