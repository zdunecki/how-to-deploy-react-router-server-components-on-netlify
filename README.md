# How to setup React Router Server Components on Netlify (Experimental RSC)

⚠️ **EXPERIMENTAL**: This template demonstrates React Server Components with React Router. This is experimental technology and not recommended for production use.

A modern template for exploring React Server Components (RSC) with React Router, powered by Vite.

## Features

- 🧪 **Experimental React Server Components**
- 🚀 Server-side rendering with RSC
- ⚡️ Hot Module Replacement (HMR)
- 📦 Asset bundling and optimization with Vite
- 🔄 Data loading and mutations
- 🔒 TypeScript by default
- 🎉 TailwindCSS for styling
- 📖 [React Router docs](https://reactrouter.com/)
- 📚 [React Server Components guide](https://reactrouter.com/how-to/react-server-components)

## Getting Started

### Installation

Install the dependencies:

```bash
npm install
```

### Development

Start the development server with HMR:

```bash
npm run dev
```

Your application will be available at `http://localhost:5173`.

## Building for Production

Create a production build:

```bash
npm run build
```

## Running Production Build

Run the production server:

```bash
npm start
```

## Deploying to Netlify

This template is configured for seamless deployment on Netlify with React Server Components support.

### Automatic Deployment

1. **Connect your repository** to Netlify
2. **Build settings** are pre-configured in `netlify.toml`:
   - Build command: `npm run build`
   - Publish directory: `dist/client`
   - Functions directory: `dist/rsc`

3. **Deploy** - Netlify will automatically build and deploy your app

### Netlify Configuration

The `netlify.toml` file includes:

- **Build settings** for React Server Components
- **Redirect rules** to handle RSC routing
- **Function configuration** for server-side rendering

### Important Notes

- ⚠️ **Experimental**: React Server Components on Netlify is experimental
- 🔧 **Functions**: RSC requires Netlify Functions for server-side rendering
- 🌐 **Edge Functions**: Consider using Netlify Edge Functions for better performance
- 📊 **Monitoring**: Monitor function execution times and cold starts

### Troubleshooting

- **Build failures**: Ensure all dependencies are in `package.json`
- **Function timeouts**: Optimize server-side code for faster execution
- **Routing issues**: Check redirect rules in `netlify.toml`

## Understanding React Server Components

This template includes three entry points:

- **`entry.rsc.tsx`** - React Server Components entry point
- **`entry.ssr.tsx`** - Server-side rendering entry point  
- **`entry.browser.tsx`** - Client-side hydration entry point

Learn more about React Server Components with React Router in our [comprehensive guide](https://reactrouter.com/how-to/react-server-components).

## Styling

This template comes with [Tailwind CSS](https://tailwindcss.com/) already configured for a simple default starting experience. You can use whatever CSS framework you prefer.

---

Built with ❤️ using React Router. 