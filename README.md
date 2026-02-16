# Portfolio - Frontend Only

A beautiful, fully-frontend portfolio built with React, TypeScript, and Tailwind CSS. All data is stored statically without any backend or database requirements.

## Features

- ✨ Stunning animations with Framer Motion
- 📱 Fully responsive design
- 🎨 Modern UI with Tailwind CSS and shadcn/ui components
- ⚡ Lightning-fast static site generation
- 🔍 Optimized for search engines
- ♿ Accessible components with ARIA support

## Project Structure

```
client/src/
├── components/        # React components (Projects, Skills, Experience, etc.)
├── data/             # Static data files
│   ├── projects.ts   # Project information
│   ├── skills.ts     # Skills and proficiency levels
│   └── experience.ts # Career and education history
├── types/            # TypeScript type definitions
├── hooks/            # Custom React hooks
├── pages/            # Page components
└── lib/              # Utilities and helpers
```

## Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Installation

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

3. Open your browser and navigate to `http://localhost:5173`

## Customizing Your Data

### Edit Projects
Edit `/client/src/data/projects.ts` to add/modify your projects:
```typescript
export const PROJECTS_DATA = [
  {
    id: 1,
    title: "Your Project",
    shortDescription: "...",
    // ... other fields
  }
];
```

### Edit Skills
Edit `/client/src/data/skills.ts` to customize your skills:
```typescript
export const SKILLS_DATA = [
  { id: 1, name: "React", category: "frontend", proficiency: 95 },
  // ... more skills
];
```

### Edit Experience
Edit `/client/src/data/experience.ts` to add your career history:
```typescript
export const EXPERIENCE_DATA = [
  {
    id: 1,
    role: "Your Role",
    company: "Company Name",
    duration: "2023 - Present",
    // ... other fields
  }
];
```

### Update Contact Email
Update the email address in `/client/src/components/Contact.tsx` and `/client/src/hooks/use-portfolio.ts`:
- Replace `hello@dwarakesh.dev` with your email address

## Building for Production

Build the optimized production version:
```bash
npm run build
```

Preview the production build locally:
```bash
npm run preview
```

The built files will be in the `dist/public` directory, ready to be deployed anywhere.

## Deployment

This is a static site and can be deployed to any static hosting service:

- **Vercel** (recommended): Connect your GitHub repo to Vercel for automatic deployments
- **Netlify**: Drop the `dist/public` folder or connect your repo
- **GitHub Pages**: Push to a `gh-pages` branch
- **Any CDN**: Serve the `dist/public` folder

## Tech Stack

- **React** 18 - UI library
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling
- **Framer Motion** - Animations
- **Vite** - Build tool
- **shadcn/ui** - Component library

## No Backend Required

This portfolio is completely frontend-based:
- ✅ No server needed
- ✅ No database required
- ✅ No API calls
- ✅ Contact form opens email client
- ✅ All data is static and fast to load

## License

MIT - feel free to use this portfolio as a template for your own!
