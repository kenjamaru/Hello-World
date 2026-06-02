# Hello World - Next.js 14+ Application

A simple, responsive "Hello World" website built with **Next.js 14+** using the **App Router** and **vanilla CSS** (no Tailwind or CSS-in-JS libraries).

## 📋 Project Structure

```
Hello-World/
├── app/
│   ├── layout.tsx          # Root layout component with metadata
│   ├── page.tsx            # Main home page component
│   └── globals.css         # Global styles with CSS variables
├── package.json            # Project dependencies and scripts
├── tsconfig.json           # TypeScript configuration
├── next.config.js          # Next.js configuration
├── .gitignore              # Git ignore rules
└── README.md               # This file
```

## 📝 File Descriptions

### **app/layout.tsx**
- Root layout component for the entire application
- Defines metadata (title, description, keywords)
- Sets up HTML structure and common head tags
- Wraps all pages with consistent layout

### **app/page.tsx**
- Main home page component
- Displays the "Hello, World!" heading
- Includes a description paragraph
- Semantic HTML structure with CSS classes

### **app/globals.css**
- Central styling file for the entire application
- Defines CSS variables for colors, fonts, spacing, and transitions
- Includes base reset and normalization
- Responsive breakpoints for mobile, tablet, and desktop
- Smooth animations (fade-in, fade-in-up effects)
- Hover effects on heading with gradient
- Dark mode support using `prefers-color-scheme`
- Accessibility features (focus states)

### **package.json**
- Project metadata and description
- npm scripts for development and production
- Dependencies: React 18+, Next.js 14+
- DevDependencies: TypeScript, ESLint config

### **tsconfig.json**
- TypeScript compiler configuration
- Strict mode enabled for better type safety
- Path aliases configured (@/* for imports)
- Bundler mode for Next.js compatibility

### **next.config.js**
- Next.js configuration
- React strict mode enabled for development

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ and npm (or yarn, pnpm)

### Installation & Running

1. **Clone the repository** (if not already done)
   ```bash
   git clone https://github.com/kenjamaru/Hello-World.git
   cd Hello-World
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   ```

3. **Run development server**
   ```bash
   npm run dev
   # or
   yarn dev
   # or
   pnpm dev
   ```

4. **Open your browser**
   - Navigate to `http://localhost:3000`
   - You should see the "Hello, World!" page

### Build for Production

```bash
npm run build
npm start
```

## 🎨 Features

### Styling
- ✅ **CSS Variables**: Centralized color, font, and spacing management
- ✅ **Responsive Design**: Mobile-first approach with breakpoints at 480px, 768px, and 1024px
- ✅ **Dark Mode Support**: Automatically adapts to system color scheme preference
- ✅ **Animations**: Smooth fade-in and fade-in-up effects
- ✅ **Hover Effects**: Heading scales and adds shadow on hover
- ✅ **Gradient Text**: Modern gradient effect on the main heading

### Accessibility
- ✅ Semantic HTML5 structure
- ✅ Focus states for keyboard navigation
- ✅ Proper heading hierarchy
- ✅ Good color contrast ratios
- ✅ Print-friendly styles

### Performance
- ✅ Vanilla CSS (no extra dependencies)
- ✅ Minimal JavaScript
- ✅ Optimized for Core Web Vitals
- ✅ Fast initial load

## 🛠️ Development

### Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server (hot reload) |
| `npm run build` | Build for production |
| `npm start` | Start production server |
| `npm run lint` | Run ESLint to check code quality |

### Customization

#### Change Colors
Edit CSS variables in `app/globals.css`:
```css
:root {
  --color-primary: #1a1a1a;
  --color-accent: #0066cc;
  --color-background: #ffffff;
  --color-text: #333333;
}
```

#### Modify Fonts
Update font family variable:
```css
--font-primary: 'Your Font Here', sans-serif;
```

#### Adjust Heading Size
Change in the `:root` selector or media queries:
```css
--font-size-heading: 48px;
```

## 📱 Responsive Breakpoints

| Device | Breakpoint | Heading Size |
|--------|-----------|--------------|
| Mobile | < 480px | 36px |
| Tablet | 768px - 1023px | 56px |
| Desktop | > 1024px | 64px |

## ♿ Accessibility Features

- ✅ Focus visible outlines (blue accent color)
- ✅ Semantic HTML elements
- ✅ Proper heading hierarchy (single h1)
- ✅ Readable line heights and letter spacing
- ✅ High contrast text
- ✅ Keyboard navigable

## 🌙 Dark Mode

The application automatically detects user's system preference using `prefers-color-scheme` media query. Colors adapt automatically when dark mode is enabled.

## 📦 Dependencies

### Production
- **React**: ^18.2.0 - UI library
- **React DOM**: ^18.2.0 - React rendering for web
- **Next.js**: ^14.0.0 - React framework with SSR/SSG

### Development
- **TypeScript**: ^5.3.0 - Static type checking
- **ESLint**: ^8.55.0 - Code quality linter
- **ESLint Config Next**: ^14.0.0 - Next.js specific ESLint rules

## 📄 License

This project is open source and available for educational and personal use.

## 💡 Tips

1. **No CSS Framework**: This project intentionally uses vanilla CSS to demonstrate pure styling capabilities
2. **Type Safety**: TypeScript is configured for strict mode - catch errors early
3. **CSS Organization**: CSS is organized in sections with clear comments for easy navigation
4. **Production Ready**: All files are production-ready with best practices applied

## 🤝 Contributing

Feel free to fork this project and make improvements!

---

**Created**: 2026-06-02  
**Next.js Version**: 14+  
**Node Version**: 18+
