# Tarea 2 – Práctica: Construcción de repositorio y creación de una línea base (Baseline v1.0)  
**Frecuente 1 – Parcial I | Semana 2**

**Autor:** Christian Felipe Torres López  

---

## 📌 Descripción del trabajo

En esta práctica se organiza un repositorio como **depósito de elementos de configuración** y se establece una **línea base (Baseline v1.0)** utilizando buenas prácticas de control de versiones con Git, mediante el uso de **tags** y un **release**.

El objetivo principal es que el repositorio sea **reproducible, auditable y con trazabilidad**, permitiendo identificar claramente qué elementos fueron aprobados como línea base y cómo se gestionan los cambios posteriores.

---

## 🎯 Objetivo de la actividad

Implementar un repositorio como depósito de elementos de configuración y crear una línea base (Baseline v1.0), aplicando buenas prácticas de versionado, estructura, evidencias y control mínimo de cambios, para comprender su impacto en la **calidad**, **trazabilidad** y **confiabilidad** del software.

---

## ✅ Requisitos previos

- Git instalado.
- Cuenta en GitHub o GitLab (repositorio público o privado).
- Editor de código (VS Code recomendado).
- Conocimientos básicos de control de versiones.

> 💡 **Tip docente:** Si el repositorio no puede reconstruirse exactamente desde un tag, entonces no es un *release*, es solo una anécdota.

---

## 🗂️ Estructura del repositorio

```text
GCS_Semana2_Baseline_TorresChristian/
│
├── docs/
│   ├── SRS/
│   │   └── SRS_v1.md
│   └── SDD/
│       └── SDD_v1.md
│
├── src/
│   └── main.py
│
├── tests/
│   └── test_placeholder.md
│
├── config/
│   └── config.example
│
├── scripts/
│
├── CHANGELOG.md
└── README.md


# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:

```js
export default defineConfig([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...

      // Remove tseslint.configs.recommended and replace with this
      tseslint.configs.recommendedTypeChecked,
      // Alternatively, use this for stricter rules
      tseslint.configs.strictTypeChecked,
      // Optionally, add this for stylistic rules
      tseslint.configs.stylisticTypeChecked,

      // Other configs...
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
])
```

You can also install [eslint-plugin-react-x](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-x) and [eslint-plugin-react-dom](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-dom) for React-specific lint rules:

```js
// eslint.config.js
import reactX from 'eslint-plugin-react-x'
import reactDom from 'eslint-plugin-react-dom'

export default defineConfig([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...
      // Enable lint rules for React
      reactX.configs['recommended-typescript'],
      // Enable lint rules for React DOM
      reactDom.configs.recommended,
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
])
```
