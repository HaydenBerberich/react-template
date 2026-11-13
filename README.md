# React Template

A reusable starter template for building React applications with Vite. It includes client-side routing, CSS Modules, linting, and a testing setup with Vitest and React Testing Library.

## Tech Stack

- **React 19** – Component-based UI development
- **Vite 8** – Development server and production build tooling
- **React Router 8** – Client-side routing
- **CSS Modules** – Component-scoped styles
- **Vitest** – Test runner
- **React Testing Library** – Component and user-interaction testing
- **ESLint** – JavaScript, React Hooks, and React Refresh linting
- **React Compiler** – Enabled through the Vite Babel plugin

## Getting Started

### Prerequisites

- Node.js (current LTS version recommended)
- npm

### Installation

Clone the repository and install its dependencies:

```bash
git clone https://github.com/HaydenBerberich/react-template.git
cd react-template
npm install
```

### Start the Development Server

```bash
npm run dev
```

Vite will print the local development URL in the terminal.

## Available Scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the Vite development server |
| `npm run build` | Create an optimized production build in `dist/` |
| `npm run preview` | Preview the production build locally |
| `npm test` | Run tests with Vitest |
| `npm run lint` | Run ESLint |

## Project Structure

```
react-template/
├── public/             # Static assets
├── src/
│   ├── App.jsx         # Root application component
│   ├── App.module.css  # Component-scoped styles
│   ├── index.css       # Global styles
│   ├── main.jsx        # Application entry point
│   └── routes.jsx      # React Router route configuration
├── tests/
│   └── setup.js        # Vitest and Testing Library setup
├── eslint.config.js    # ESLint configuration
├── index.html
├── package.json
└── vite.config.js      # Vite and Vitest configuration
```

## Routing

Routes are defined in `src/routes.jsx` and passed to React Router's `createBrowserRouter` in `src/main.jsx`. Add or modify route objects in that file as the application grows.

## Styling

Use `.module.css` files for component-specific styles. The `src/index.css` file is imported by the application entry point and is intended for global styles and resets.

## Testing

Tests run with Vitest in a jsdom environment. React Testing Library and the `jest-dom` matchers are configured in `tests/setup.js`.

Run the test suite with:

```bash
npm test
```

## Building

Create a production build with:

```bash
npm run build
```

The generated files are placed in `dist/`. To serve that build locally, run `npm run preview`.
