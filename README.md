# Portfolio Website

A modern, shareable portfolio website built with Next.js, TypeScript, and Tailwind CSS. Perfect for showcasing your achievements, experience, and projects.

## Features

✨ **Modern Design** - Beautiful, responsive UI with smooth animations
📝 **Easy Content Management** - Update your portfolio by editing JSON files
⚡ **Performance Optimized** - Fast load times and smooth interactions
📱 **Mobile Responsive** - Works perfectly on all devices
🚀 **GitHub Pages Ready** - Deploy automatically with GitHub Actions
🎯 **SEO Friendly** - Built-in Next.js optimizations

## Sections

- **Hero** - Eye-catching landing section
- **Experience** - Work history and career timeline
- **Skills** - Technical expertise organized by category
- **Certifications** - Awards and professional credentials
- **Projects** - Portfolio work with case studies
- **Blog** - Share articles and insights
- **Contact** - Social links and contact information

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm or yarn

### Installation

```bash
# Install dependencies
npm install

# Run development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to see your portfolio.

## Customization

### Update Your Information

Edit `src/data/portfolio.json` with your information:

```json
{
  "profile": {
    "name": "Your Name",
    "title": "Your Title",
    "bio": "Your bio",
    "email": "your.email@example.com"
  },
  "experience": [...],
  "skills": [...],
  "certifications": [...],
  "projects": [...],
  "blog": [...],
  "social": [...]
}
```

### Customize Colors

Edit the theme in `tailwind.config.js`:

```js
colors: {
  primary: "#1a1a2e",
  secondary: "#16213e",
  accent: "#0f3460",
  highlight: "#e94560",
}
```

### Add Sections

Components are modular and located in `src/components/`. Add new sections by:
1. Creating a new component
2. Importing it in `src/app/page.tsx`
3. Adding data to `src/data/portfolio.json`

## Deployment

### GitHub Pages

The project is configured for GitHub Pages deployment:

1. Ensure `gh-pages` branch exists (or change to your deployment branch)
2. GitHub Actions will automatically build and deploy on `main` push
3. Your site will be live at `https://vicatugy.github.io/sturdy-train`

### Other Platforms

Deploy easily to:
- **Vercel**: Push to GitHub, connect with Vercel
- **Netlify**: Connect repository, set build command to `npm run build`
- **Custom Server**: Use `npm run build && npm start`

## Project Structure

```
sturdy-train/
├── src/
│   ├── app/               # Next.js app directory
│   ├── components/        # React components
│   ├── data/
│   │   └── portfolio.json # Your content
│   ├── lib/               # Utilities
│   └── styles/            # Global styles
├── public/                # Static assets
├── .github/workflows/     # GitHub Actions
└── tailwind.config.js     # Tailwind configuration
```

## Technologies Used

- **Next.js 14** - React framework
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling
- **PostCSS** - CSS processing

## Tips for Best Results

1. **Profile Picture** - Add a profile image to `public/profile.jpg`
2. **Project Images** - Add project images to `public/projects/`
3. **Social Links** - Update all social media links in `portfolio.json`
4. **Custom Domain** - Add a `CNAME` file to `public/` for custom domain
5. **SEO** - Update metadata in `src/app/layout.tsx`

## License

This project is open source and available under the MIT License.

## Support

For issues or questions, create an issue in the repository.

---

Built with ❤️ to help you showcase your achievements!
