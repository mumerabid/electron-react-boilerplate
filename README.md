# Electron React Boilerplate

A foundation for scalable desktop apps with **Tailwind CSS** support.

## Features

- ⚡ **Electron** - Cross-platform desktop app framework
- ⚛️ **React** - Modern UI library with hooks support
- 🎨 **Tailwind CSS** - Utility-first CSS framework for rapid UI development
- 📝 **TypeScript** - Type safety and better developer experience
- 🎯 **Sass** - CSS preprocessor support
- 📦 **Webpack** - Module bundler with hot reload
- 🔧 **ESLint** - Code linting and formatting

## Getting Started

### Prerequisites

- Node.js (version 14 or higher)
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/electron-react-boilerplate/electron-react-boilerplate.git
   cd electron-react-boilerplate
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

## Tailwind CSS Support

This boilerplate comes pre-configured with **Tailwind CSS** for rapid UI development:

- ✅ PostCSS and Autoprefixer configured
- ✅ Tailwind config with custom colors (sky, cyan)
- ✅ Works in both development and production builds
- ✅ Hot reload support for Tailwind classes

### Using Tailwind CSS

Simply use Tailwind utility classes in your React components:

```tsx
function MyComponent() {
  return (
    <div className="bg-blue-500 text-white p-6 rounded-lg shadow-lg">
      <h1 className="text-2xl font-bold mb-4">Hello Tailwind!</h1>
      <button className="bg-white text-blue-500 px-4 py-2 rounded hover:bg-blue-50">
        Click me
      </button>
    </div>
  );
}
```

### Customizing Tailwind

Edit `tailwind.config.js` to customize your design system:

```js
module.exports = {
  content: ['./src/renderer/**/*.{js,jsx,ts,tsx,ejs}'],
  theme: {
    extend: {
      colors: {
        brand: {
          primary: '#your-color',
          secondary: '#your-color',
        },
      },
    },
  },
  plugins: [],
};
```

## Scripts

- `npm start` - Start development server
- `npm run build` - Build for production
- `npm run package` - Package the app for distribution
- `npm run lint` - Run ESLint
- `npm run lint:fix` - Fix ESLint errors

## Project Structure

```
├── src/
│   ├── main/           # Electron main process
│   └── renderer/       # React renderer process
├── assets/             # Static assets
├── .erb/               # Build configuration
├── tailwind.config.js  # Tailwind CSS configuration
└── package.json
```

## Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Electron React Boilerplate](https://github.com/electron-react-boilerplate/electron-react-boilerplate) - Original boilerplate
- [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework
- [React](https://reactjs.org/) - UI library
- [Electron](https://electronjs.org/) - Desktop app framework
