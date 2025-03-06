# React + Tailwind + React Router Starter

A lightweight, modern starter template for building React applications with Tailwind CSS and React Router.

## Features

- ⚡️ [React](https://reactjs.org/) - A JavaScript library for building user interfaces
- 🎨 [Tailwind CSS](https://tailwindcss.com/) - A utility-first CSS framework
- 🧭 [React Router](https://reactrouter.com/) - Declarative routing for React applications
- 📦 [Vite](https://vitejs.dev/) - Next generation frontend tooling
- 🔍 ESLint + Prettier - Code quality tools
- 📱 Responsive design ready

## Getting Started

### Prerequisites

- Node.js (version 14 or later)
- npm or yarn

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/react-tailwind-react-router-starter.git
cd react-tailwind-react-router-starter
```

2. Install dependencies
```bash
npm install
# or
yarn
```

3. Start the development server
```bash
npm run dev
# or
yarn dev
```

4. Open your browser and visit `http://localhost:5173`

## Project Structure

```
/
├── public/              # Static files
├── src/
│   ├── assets/          # Images, fonts, etc.
│   ├── components/      # Reusable components
│   ├── layouts/         # Layout components
│   ├── pages/           # Page components
│   ├── routes/          # Route definitions
│   ├── styles/          # Global styles
│   ├── App.jsx          # Main component
│   ├── main.jsx         # Entry point
│   └── index.css        # Tailwind directives
├── .eslintrc.js         # ESLint configuration
├── .prettierrc          # Prettier configuration
├── index.html           # HTML template
├── postcss.config.js    # PostCSS configuration
├── tailwind.config.js   # Tailwind configuration
├── vite.config.js       # Vite configuration
└── package.json         # Dependencies and scripts
```

## Available Scripts

- `npm run dev` - Start the development server
- `npm run build` - Build for production
- `npm run preview` - Preview the production build
- `npm run lint` - Run ESLint
- `npm run format` - Format code with Prettier

## Customization

### Tailwind Configuration

You can customize your Tailwind setup in the `tailwind.config.js` file:

```js
module.exports = {
  content: ["./index.html", "./src/**/*.{js,jsx}"],
  theme: {
    extend: {
      colors: {
        // Add your custom colors here
      },
    },
  },
  plugins: [],
};
```

### Adding New Routes

Edit the routes in `src/routes/index.jsx`:

```jsx
import { createBrowserRouter } from "react-router-dom";
import Home from "../pages/Home";
import About from "../pages/About";
import NotFound from "../pages/NotFound";

const router = createBrowserRouter([
  {
    path: "/",
    element: <Home />,
  },
  {
    path: "/about",
    element: <About />,
  },
  {
    path: "*",
    element: <NotFound />,
  },
]);

export default router;
```

## Deployment

Build your application for production:

```bash
npm run build
# or
yarn build
```

The build artifacts will be stored in the `dist/` directory, ready to be deployed to your preferred hosting platform.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [React](https://reactjs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [React Router](https://reactrouter.com/)
- [Vite](https://vitejs.dev/)