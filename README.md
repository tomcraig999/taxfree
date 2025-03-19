# Offshore Portal

A Next.js-based web application for offshore company formation services.

## Features

- Modern UI with responsive design
- Static site generation for fast loading
- Easy deployment to GitHub Pages or any static hosting service

## Development

### Prerequisites

- Node.js (v14 or later)
- npm or yarn

### Installation

```bash
# Clone the repository
git clone <repository-url>
cd offshore-portal

# Install dependencies
npm install
```

### Development Server

```bash
npm run dev
```

This will start the development server at [http://localhost:3000](http://localhost:3000).

### Building for Production

```bash
npm run build
```

This will create an optimized production build in the `out` directory.

### Serving the Production Build Locally

```bash
npm run serve
```

This will serve the production build at [http://localhost:8080](http://localhost:8080).

## Deployment

### Deploying to GitHub Pages

The project is set up with GitHub Actions for automatic deployment to GitHub Pages. When you push changes to the `main` branch, the GitHub Actions workflow will automatically:

1. Build the Next.js app
2. Deploy the built files to the `gh-pages` branch
3. Make the site available at your GitHub Pages URL

You can also manually deploy by running:

```bash
npm run deploy
```

This will:
- Build the Next.js app
- Copy the build files to the `gh-pages` directory

After running this script, you can push the changes to the `gh-pages` branch:

```bash
git checkout gh-pages
git add .
git commit -m "Deploy to GitHub Pages"
git push origin gh-pages
```

### Deploying to Other Static Hosting Services

The static files in the `out` directory can be deployed to any static hosting service like Netlify, Vercel, or AWS S3.

## Project Structure

- `app/`: Next.js app directory containing pages and components
- `public/`: Static assets like images and fonts
- `out/`: Production build output
- `gh-pages/`: Files ready for GitHub Pages deployment

## Configuration

- `next.config.js`: Next.js configuration
- `tailwind.config.js`: Tailwind CSS configuration
- `deploy.sh`: Deployment script

## License

[MIT](LICENSE)
