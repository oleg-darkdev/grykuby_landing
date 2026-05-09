<a name="readme-top"></a>

<!-- <img align="right" alt="banner" src="/docs"> -->

# Landinng page for INFINITE MINESWEEPER application.

![Thumbnail](/docs/1.png)

_Check out the live project [_here_](https://grykuby.vercel.app/)._

## Table of Contents

* [Screenshots](#screenshots)
* [Acknowledgements](#acknowledgements)
* [Technologies](#technologies)
* [Usage](#usage)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
  * [Environment Variables Setup](#environment-variables-setup)
  * [Run The App](#run-the-app)
  * [Build](#build)
  * [Preview](#preview)
  * [Type Checking](#type-checking)
  * [Lint & Format](#lint--format)
  * [Deploy](#deploy)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



| ![Login Page](/docs/1.png) | ![Profile Page](/docs/2.png) |
|:--:|:--:|
<!-- | _Login Page_ | _Profile Page_ | -->
| ![Dashboard Page](/docs/3.png) | ![Disucussion Post & Comments](/docs/4.png) |
|:--:|:--:|
| ![Places Page](/docs/5.png) | ![Achievements Page](/docs/6.png) |
|:--:|:--:|

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 👾 Technologies

- [Typescipt](https://www.typescriptlang.org/).
- [FSD architecture](https://feature-sliced.design/ru/docs/get-started)
- [SvelteJS](https://svelte.dev/)
- [TailwindCSS](https://tailwindcss.com/)
- [SvelteKIT](https://kit.svelte.dev/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


## Prerequisites

<a name="prerequisites"></a>

Before getting started, make sure you have installed:

- Node.js >= 18
- npm >= 9

Check installed versions:

```bash
node -v
npm -v
```

---

## Installation

<a name="installation"></a>

Install dependencies:

```bash
npm install
```

---

## Environment Variables Setup


<a name="environment-variables-setup"></a>

Create a `.env` file in the project root:

```env
PUBLIC_API_URL=http://localhost:3000
```

Add any additional environment variables if required.

---

## Run The App


<a name="run-the-app"></a>

### Development Mode

```bash
npm run dev
```

This command runs:

- `typesafe-i18n` generation
- Vite development server

Simultaneously using `npm-run-all`.

---

### Run Only Vite

```bash
npm run start
```

Automatically opens the application in the browser using `--open`.

---

## Build



<a name="build"></a>

Production build:

```bash
npm run build
```

Builds the production-ready version of the application.

---

## Preview

<a name="preview"></a>

Preview the production build locally:

```bash
npm run preview
```

Runs a local preview server for the production build.

---

## Internationalization (i18n)


Generate typesafe translations:

```bash
npm run typesafe-i18n
```

Powered by:

- `typesafe-i18n`

Features:

- fully typed translations
- autocomplete support
- protection against invalid translation keys

---

## Type Checking

<a name="type-checking"></a>

### One-time Check

```bash
npm run check
```

Runs:

- `svelte-kit sync`
- `svelte-check`

---

### Watch Mode

```bash
npm run check:watch
```

Continuously watches and reports TypeScript/Svelte errors.

---

## Deploy

<a name="deploy"></a>


### Initial Server Setup

```bash
npm run deploy:setup
```

Uses:

```bash
pm2 deploy production setup
```

---

### Deploy Application

```bash
npm run deploy
```

Uses the PM2 deployment pipeline:

```bash
pm2 deploy production
```


## 💪🏼 Show your support

Give a ⭐️ if you like our stuff!


<p align="right">(<a href="#readme-top">back to top</a>)</p>
