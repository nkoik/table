# React Table

This is a React application created with Vite + Tailwind + Vitest for testing.

# Component Structure and Naming Conventions

We follow specific patterns and naming conventions in this project to ensure consistency and readability.

#### Patterns

We use the Presentational-Container pattern along with React hooks. This means that we separate our components into two categories:

1. **Presentational Components**: These are components that are primarily concerned with how things look. They usually have some DOM markup and styles and they receive data and callbacks exclusively via props.

2. **Container Components**: These are components that are more concerned with how things work. They provide the data and behavior to presentational or other container components.

We use [Tailwind CSS](https://tailwindcss.com/) for styling our components. Avoid using global classes; instead, use utility classes to style your components.

#### Naming Conventions

- **View/Layout Components**: These should be suffixed with `Page`. For example, `TablePage`, `InnerPage`.

- **Stateful/Heavy Calculation Components**: Any component that communicates with the state management module (if one exists) or performs heavy calculations should be suffixed with `Container`. For example, `CustomerContainer`.

- **Styling Components**: Any component that serves only as a style template should be suffixed with `Wrapper`. For example, `StepWrapper`.

- **Skeleton Components**: These should be named like `ComponentNameSkeleton`. For example, `TableSkeleton`, `CustomerSkeleton`.

- **Other Components**: Any other component can be used as a presentational component or with small state data can be named as you want.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- You have installed [Node.js and npm](https://nodejs.org/en/download/) - prefer nvm 18.18.0

## Installing

To install, follow these steps:

1. Clone the repository:

```bash
git clone https://github.com/nkoik/table.git
```

2. Install the project dependencies:

```bash
npm ci
```

### Using React Table

1. Start the development server:

```bash
npm run dev
```

Open your web browser and visit http://localhost:8080

2. Build the app

```bash
npm run build
```
