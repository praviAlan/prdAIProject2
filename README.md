# p5.js Interactive Portfolio

A visually engaging portfolio website showcasing 11 interactive p5.js sketches. This is not just a portfolio—it's a playable gallery where visitors can experience creative coding projects directly in their browser.

## 🎨 Features

- **Interactive Gallery**: Browse 11 unique p5.js projects with animated previews
- **Live Canvas**: Each project runs directly in the browser—no setup required
- **Dark Mode**: Beautiful dark theme optimized for visual artwork
- **Responsive Design**: Works smoothly on desktop, tablet, and mobile
- **Fast Loading**: Performance-optimized with lazy loading
- **About Section**: Learn about the creator and exploration areas

## 🚀 Tech Stack

- **Framework**: [Next.js](https://nextjs.org/) 14+
- **Library**: [p5.js](https://p5js.org/)
- **Language**: JavaScript (React)
- **Styling**: CSS3 with gradients and animations
- **Hosting**: Vercel / GitHub Pages

## 📋 Projects Included

1. **Particle System** - Interactive particle effects responding to mouse
2. **Generative Landscape** - Procedurally generated terrain
3. **Interactive Mandelbrot** - Zoomable Mandelbrot set visualization
4. **Perlin Noise Walker** - Smooth organic motion patterns
5. **Flocking Simulation** - Emergent bird-like behavior
6. **Reactive Canvas** - Audio-responsive generative patterns
7. **Bouncing Balls** - Physics simulation with collisions
8. **Cellular Automata** - Conway's Game of Life
9. **Network Visualization** - Dynamic network graph
10. **Recursive Fractals** - Beautiful fractal trees
11. **Interactive Creatures** - Soft-body creature animations

## 💻 Getting Started

### Prerequisites

- Node.js 16+ and npm (or yarn/pnpm)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/p5js-portfolio.git
   cd p5js-portfolio
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run development server**
   ```bash
   npm run dev
   ```
   Open [http://localhost:3000](http://localhost:3000) in your browser

4. **Build for production**
   ```bash
   npm run build
   npm start
   ```

## 📁 Project Structure

```
.
├── app/
│   ├── layout.js              # Root layout
│   ├── page.js                # Home/Gallery page
│   ├── page.css               # Gallery styles
│   ├── globals.css            # Global styles
│   ├── about/
│   │   ├── page.js            # About page
│   │   └── about.css          # About styles
│   └── projects/
│       └── [id]/
│           ├── page.js        # Project detail page
│           └── project.css    # Project styles
├── package.json
├── next.config.js
├── jsconfig.json
├── vercel.json
├── .gitignore
├── .vercelignore
└── README.md
```

## 🎮 Customization

### Adding New Projects

Edit `app/page.js` to add projects to the gallery grid:

```javascript
const projects = [
  {
    id: 1,
    title: 'Your Project Title',
    description: 'Short description of what it does',
    tags: ['Tag1', 'Tag2'],
    icon: '🎨',
  },
  // ...
];
```

Then update `app/projects/[id]/page.js` with the sketch logic for that project ID.

### Customizing Sketches

Each project's sketch is defined in the `switch` statement in `app/projects/[id]/page.js`. Modify or add new sketch functions:

```javascript
const drawYourProject = (p) => {
  // Your p5.js code here
  p.background(10, 14, 39);
  p.fill(0, 191, 255);
  p.ellipse(p.mouseX, p.mouseY, 50);
};
```

### Updating Styling

- **Global styles**: Edit `app/globals.css`
- **Dark mode colors**: Change the color values (default: `#0a0e27` background, `#00bfff` accent)
- **Typography**: Modify font sizes and families in respective CSS files

## 🚀 Deployment

### Deploy to Vercel (Recommended)

1. **Push to GitHub**
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

2. **Connect to Vercel**
   - Go to [https://vercel.com](https://vercel.com)
   - Sign in with GitHub
   - Click "Add New" → "Project"
   - Select your repository
   - Click "Deploy"

3. **Done!** Your portfolio is live at your Vercel URL

### Deploy to GitHub Pages

1. Update `next.config.js`:
   ```javascript
   const nextConfig = {
     output: 'export',
     reactStrictMode: true,
   };
   ```

2. Build and deploy:
   ```bash
   npm run build
   # Push the out/ folder to gh-pages branch
   ```

## 📊 Performance

- **Page load time**: < 2 seconds
- **Sketch performance**: Optimized for 60 FPS
- **Bundle size**: ~50KB gzipped (p5.js: ~35KB)

## 🔧 Configuration

### Environment Variables

Create `.env.local` if needed:
```
NEXT_PUBLIC_GITHUB_URL=https://github.com/yourusername
NEXT_PUBLIC_SITE_URL=https://yourportfolio.com
```

### Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 🎓 Learning Resources

- [p5.js Documentation](https://p5js.org/reference/)
- [Next.js Documentation](https://nextjs.org/docs)
- [Generative Art with p5.js](https://generativeart.com/)
- [Coding Train](https://www.thecodingtrainsf.com/) - Great p5.js tutorials

## 📝 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Feel free to fork, modify, and use this template for your own portfolio!

## ✉️ Contact

- **Email**: your.email@example.com
- **GitHub**: [@yourusername](https://github.com/yourusername)
- **LinkedIn**: [Your Profile](https://linkedin.com/in/yourprofile)

---

Built with ✨ and p5.js
