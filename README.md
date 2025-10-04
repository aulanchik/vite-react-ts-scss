# Vite + React + TypeScript + SCSS Boilerplate

This repository provides a minimal and clean starter template for building modern web applications. It comes pre-configured with a powerful stack to get you up and running quickly.

## Features

-   **Vite:** Next-generation frontend tooling for an extremely fast development experience.
-   **React 19:** The latest version of the React library for building user interfaces.
-   **TypeScript:** Static type-checking to enhance code quality and developer productivity.
-   **SCSS:** A pre-configured, structured setup for styling with Sass.
-   **Linting:** ESLint configured for TypeScript and React to enforce code quality.
-   **Formatting:** Prettier for consistent and automatic code formatting.
-   **Absolute Imports:** Pre-configured path alias `@/` pointing to the `src` directory for cleaner import statements.
-   **Dependabot:** Automated dependency management to keep your project up-to-date.

## Getting Started

To use this template, clone the repository and install the necessary dependencies.

### Prerequisites

-   Node.js (LTS version recommended)
-   npm, pnpm, or yarn

### Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/aulanchik/vite-react-ts-scss.git
    ```

2.  Navigate to the project directory:
    ```bash
    cd vite-react-ts-scss
    ```

3.  Install dependencies:
    ```bash
    npm install
    ```

## Available Scripts

This project includes several scripts to help with your development workflow:

-   **`npm run dev`**
    Starts the development server with Hot Module Replacement (HMR) enabled.

-   **`npm run build`**
    Checks types with TypeScript and bundles the application for production into the `dist` folder.

-   **`npm run lint`**
    Runs ESLint to analyze the code for potential errors and style issues.

-   **`npm run preview`**
    Serves the production build locally to preview your application as it will appear in deployment.

## Project Structure

The project is organized with a focus on scalability and maintainability.

```
└── src/
    ├── assets/
    │   └── styles/
    │       ├── _base.scss       # Base styles, resets
    │       ├── _variables.scss  # SCSS variables (colors, fonts, etc.)
    │       └── index.scss       # Main entry point for styles
    ├── App.tsx                  # Main App component
    └── main.tsx                 # Application entry point
```

-   **`src/assets/styles`**: Contains global SCSS files. `index.scss` imports all other partials and is imported once in `main.tsx`.
-   **`vite.config.ts`**: Configures Vite, including the `@/` path alias.
-   **`tsconfig.json`**: TypeScript configuration, including strict mode and the `@/` path alias.
