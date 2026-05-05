# 📦 Web App Structure (FSD)

## 📚 Overview

This project follows the **Feature-Sliced Design (FSD)** architecture:
[https://feature-sliced.design/ru/docs/get-started](https://feature-sliced.design/ru/docs/get-started)

FSD helps organize code by responsibility and scalability by dividing the logic into layers such as `widgets`, `entities`, and `shared`.

---

## 🗂 Project Structure

```
src/
└── lib/
    ├── widgets/
    │   └── landing/
    │       ├── index.ts
    │       ├── Cta.svelte
    │       ├── Faq.svelte
    │       ├── Features.svelte
    │       ├── Footer.svelte
    │       ├── Gallery.svelte
    │       └── Hero.svelte
    │
    ├── entities/
    │   └── landing/
    │       └── index.ts
    │
    └── shared/
        └── data/
            ├── index.ts
            ├── faq.ts
            ├── tags.ts
            ├── navigation.ts
            ├── social.ts
            ├── FaqCard.ts
            └── TagsLine.ts
```

---

## 🧩 Widgets Level (`/widgets/landing`)

High-level UI blocks that form pages.

| File              | Description                              |
| ----------------- | --------------------- ---------------- |
| `index.ts`        | Entry point, exports all components |
| `Cta.svelte`      | CTA component *(not used)*     |
| `Faq.svelte`      | FAQ section                            |
| `Features.svelte` | Description of features                 |
| `Footer.svelte`   | Footer of the 




## 📊 Shared Layer (`/shared/data`)

Data and basic reusable components.

### 📁 Data

| File            | Description           |
| --------------- | ------------------ |
| `faq.ts`        | Data for FAQ     |
| `tags.ts`       | Keywords     |
| `navigation.ts` | Navigation (header) |
| `social.ts`     | Social links  |

### 🧩 Components

| File          | Description     |
| ------------- | ------------ |
| `FaqCard.ts`  | FAQ Card |
| `TagsLine.ts` | Tag Line  |

---

## 🔄 Component Dependencies

```
Widgets
 ├── Faq.svelte
 │    ├── uses → FaqCard
 │    └── uses → TagsLine
 │
 ├── Features.svelte
 │    └── uses → TagsLine
 │
 ├── Footer.svelte
 │    └── uses → social.ts
 │
 └── Hero.svelte
      └── uses → navigation.ts
```

Translated with DeepL.com (free version)