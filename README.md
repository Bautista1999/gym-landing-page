# Gym Landing Page

A modern, responsive landing page for fitness businesses built with SvelteKit and Tailwind CSS.

## Features

- Hero section with compelling fitness imagery
- Services showcase with detailed descriptions
- Membership pricing plans
- Customer testimonials
- Contact information and location
- Fully responsive design
- Modern UI with smooth animations

## Tech Stack

- **SvelteKit** - Full-stack web framework
- **Tailwind CSS** - Utility-first CSS framework
- **Vite** - Build tool and development server

## Quick Start

### Installation

```bash
# Clone the repository
git clone <repository-url>
cd gym-landing

# Install dependencies
npm install

# Start development server
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) to view the site.

### Build for Production

```bash
npm run build
npm run preview
```

## Customization

### Changing Colors
- Edit `tailwind.config.js` to modify the color palette
- Primary colors are defined using CSS custom properties in `app.css`
- Update brand colors by modifying the `colors` section in Tailwind config

### Updating Content
- **Hero Section**: Edit `src/lib/components/Hero.svelte`
- **Services**: Modify `src/lib/components/Services.svelte`
- **Pricing**: Update `src/lib/components/Pricing.svelte`
- **Testimonials**: Edit `src/lib/components/Testimonials.svelte`
- **Footer**: Modify `src/lib/components/Footer.svelte`

### Modifying Sections
- Add new sections by creating components in `src/lib/components/`
- Import and include them in `src/routes/+page.svelte`
- Adjust layout and styling using Tailwind classes

## Vercel Deployment

### Quick Deploy
1. Push your code to GitHub
2. Connect your GitHub repository to Vercel
3. Deploy automatically with zero configuration

### Manual Deploy
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel --prod
```

### Environment Setup
- Framework Preset: SvelteKit
- Build Command: `npm run build`
- Output Directory: `build`

## Live Demo

[View Demo](https://gym-landing-page-bautista1999s-projects.vercel.app/)

## License

MIT License