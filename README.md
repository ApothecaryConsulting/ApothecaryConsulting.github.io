# Flarze Technologies Website

Official website for Flarze Technologies - AI & Data Solutions

## 🚀 Tech Stack

- **Framework**: [Astro](https://astro.build) v5.1.5
- **Styling**: Scoped CSS with component-based architecture
- **Deployment**: GitHub Pages via GitHub Actions
- **Domain**: flarzetechnologies.com

## 📁 Project Structure

```
/
├── public/
│   └── CNAME              # Custom domain configuration
├── src/
│   ├── components/        # Reusable Astro components
│   │   ├── Header.astro
│   │   ├── Hero.astro
│   │   ├── ServiceCard.astro
│   │   ├── TeamCard.astro
│   │   └── Footer.astro
│   ├── data/              # Content data files
│   │   ├── services.ts
│   │   ├── team.ts
│   │   └── contact.ts
│   ├── layouts/
│   │   └── Layout.astro   # Base HTML layout
│   └── pages/
│       └── index.astro    # Main page
├── .github/
│   └── workflows/
│       └── deploy.yml     # GitHub Actions deployment
└── package.json
```

## 🛠️ Development

### Prerequisites

- Node.js 20+ and npm

### Commands

| Command           | Action                                       |
|:------------------|:---------------------------------------------|
| `npm install`     | Install dependencies                         |
| `npm run dev`     | Start local dev server at `localhost:4321`   |
| `npm run build`   | Build production site to `./dist/`           |
| `npm run preview` | Preview build locally before deploying       |

### Local Development

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

Visit `http://localhost:4321` to see your site.

## 📝 Updating Content

### Services

Edit `src/data/services.ts` to add/modify services:

```typescript
{
  icon: "🤖",
  title: "Service Name",
  description: "Service description",
  tools: "Tool1, Tool2, Tool3"
}
```

### Team Members

Edit `src/data/team.ts` to add/modify team members:

```typescript
{
  name: "Name",
  role: "Role",
  description: "Bio",
  imageUrl: "https://..."
}
```

### Contact Links

Edit `src/data/contact.ts` to modify contact buttons.

## 🚀 Deployment

The site automatically deploys to GitHub Pages when you push to the `main` branch.

### First-Time Setup

1. Go to your GitHub repository settings
2. Navigate to **Pages** section
3. Under **Source**, select **GitHub Actions**
4. Push to `main` branch to trigger deployment

### Manual Deployment

```bash
# Build the site
npm run build

# The dist/ folder contains the production build
# GitHub Actions will automatically deploy this
```

## 🌐 Custom Domain

The `CNAME` file in the `public/` directory configures the custom domain `flarzetechnologies.com`.

## 📦 Dependencies

- `astro` - Static site framework
- `@astrojs/check` - TypeScript checking
- `typescript` - Type safety

## 📄 License

© 2025 Flarze Technologies. All rights reserved.

