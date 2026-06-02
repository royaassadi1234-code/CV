# CV Website - Astro

A modern, responsive CV/portfolio website built with [Astro](https://astro.build) and configured for deployment on GitHub Pages.

## Features

- 🎨 Modern, responsive design with gradient styling
- 📱 Mobile-friendly layout
- 🚀 Fast performance with Astro
- 🌐 Easy GitHub Pages deployment
- 📝 Customizable CV content sections
- 🏷️ Skills tags and project cards

## Project Structure

```
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions workflow for auto-deployment
├── src/
│   ├── layouts/
│   │   └── Layout.astro        # Main layout component with styling
│   └── pages/
│       └── index.astro         # CV content page
├── public/                      # Static assets
├── astro.config.mjs            # Astro configuration
└── package.json                # Project dependencies
```

## Getting Started

### Prerequisites

- Node.js 18+ and npm

### Installation

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

The site will be available at `http://localhost:3000`

## Customizing Your CV

Edit `src/pages/index.astro` to add your personal information:

1. **Header Information**
   - Replace "Your Name" with your name
   - Update job title (e.g., "Full Stack Developer")
   - Add your contact information (email, phone, location, GitHub)

2. **About Section**
   - Replace the placeholder text with your professional summary

3. **Experience**
   - Add your work experience entries
   - Update job titles, companies, dates, and descriptions

4. **Education**
   - Add your educational background
   - Include degrees, institutions, and relevant coursework

5. **Skills**
   - Replace skill tags with your technical skills
   - Add or remove tags as needed

6. **Projects**
   - Add your featured projects
   - Include project descriptions and highlights

7. **Languages**
   - Update language proficiencies

## Deployment to GitHub Pages

### Step 1: Update Astro Config

Edit `astro.config.mjs` and replace `YOUR_GITHUB_USERNAME` with your actual GitHub username:

```javascript
site: 'https://YOUR_GITHUB_USERNAME.github.io',
```

If your repository is NOT named `YOUR_USERNAME.github.io`, also uncomment and update:

```javascript
base: '/repository-name',
```

### Step 2: Push to GitHub

1. Create a new repository on GitHub named `YOUR_USERNAME.github.io`
   - Or use any repository name and uncomment the `base` setting above

2. Push your code to the repository:
```bash
git add .
git commit -m "Initial commit: CV website"
git push origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository settings
2. Navigate to **Pages** (on the left sidebar)
3. Under "Build and deployment":
   - Select **Source**: "GitHub Actions"
4. The workflow will automatically deploy on every push to `main` branch

### Step 4: View Your Site

Your CV will be available at:
- `https://YOUR_USERNAME.github.io/` (if using `YOUR_USERNAME.github.io` repo)
- `https://YOUR_USERNAME.github.io/repository-name/` (if using another repo name)

## Build for Production

```bash
npm run build
```

This generates a static site in the `dist/` folder ready for deployment.

## Available Commands

```bash
npm run dev        # Start development server
npm run build      # Build for production
npm run preview    # Preview production build locally
```

## Styling

The CV uses a beautiful purple gradient theme with:
- Responsive grid layouts
- Mobile-first design
- Color-coded sections with border accents
- Professional typography

To customize colors, edit the CSS in `src/layouts/Layout.astro`.

## Tips

- **Print-friendly**: The site is optimized for printing. Use your browser's print function to save as PDF
- **SEO**: Update the meta description and other meta tags as needed
- **Favicon**: Replace `public/favicon.svg` and `public/favicon.ico` with your own
- **Performance**: The site is pre-optimized for speed with Astro

## Support

For more information:
- [Astro Documentation](https://docs.astro.build)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Astro Deployment Guide](https://docs.astro.build/en/guides/deploy/)

## License

This project is open source and available for personal use.
