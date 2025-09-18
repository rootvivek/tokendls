# 🎨 Figma Sync - Design Token Bridge

A React application that bridges Figma design tokens to your codebase using GitHub as an intermediary.

## 📁 Project Structure

```
figma-sync/
├── 📁 components/           # React Components
│   └── Frame25_7.jsx       # Main car card component
├── 📁 docs/                # Documentation
│   └── GITHUB_BRIDGE_GUIDE.md
├── 📁 scripts/             # Automation Scripts
│   ├── check-tokens.js     # Check Figma API tokens
│   ├── export-tokens-for-github.js
│   ├── fetch-frame.js      # Fetch Figma frames
│   └── fetch-tokens-from-github.js
├── 📁 src/                 # Source Code
│   └── main.jsx           # React entry point
├── 📁 tokens/              # Design Tokens
│   ├── tokens/            # Individual token files (JSON)
│   ├── tokens.js          # JavaScript module
│   ├── package.json       # Token package config
│   └── README.md          # Token documentation
├── index.html             # HTML entry point
├── package.json           # Project configuration
└── vite.config.js         # Vite configuration
```

## 🚀 Quick Start

### 1. Install Dependencies
```bash
npm install
```

### 2. Start Development Server
```bash
npm run dev
```

### 3. Export Design Tokens
```bash
npm run export-tokens
```

### 4. Fetch Tokens from GitHub
```bash
npm run fetch-github-tokens
```

## 📋 Available Scripts

| Script | Purpose |
|--------|---------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run export-tokens` | Export tokens to GitHub format |
| `npm run fetch-github-tokens` | Fetch tokens from GitHub |
| `npm run check-tokens` | Check Figma API tokens |

## 🎯 Workflow

```
Figma Design System → Export Script → GitHub Repo → Fetch Script → React Component
```

## 📚 Documentation

- [GitHub Bridge Guide](docs/GITHUB_BRIDGE_GUIDE.md) - Complete setup guide
- [Token Documentation](tokens/README.md) - Design token structure

## 🛠️ File Categories

### **Components** (`/components/`)
- React components and UI elements
- Main application components

### **Scripts** (`/scripts/`)
- Automation and utility scripts
- Figma API integration
- Token export/import tools

### **Tokens** (`/tokens/`)
- Design system tokens
- Color, typography, spacing definitions
- Component-specific tokens

### **Documentation** (`/docs/`)
- Setup guides and documentation
- API references and examples

### **Source** (`/src/`)
- Application entry points
- Main React application files

## 🔧 Configuration

### Environment Variables
Create a `.env` file in the root directory:
```bash
FIGMA_TOKEN=your_figma_token_here
TOKEN_FILE_KEY=your_figma_file_key
FRAME_FILE_KEY=your_figma_file_key
```

### GitHub Integration
1. Create a GitHub repository for your design tokens
2. Update the URL in `scripts/fetch-tokens-from-github.js`
3. Upload the `tokens/` folder to your GitHub repository

## 🎨 Design Token Structure

The project uses a comprehensive design token system:

- **Colors** - Brand colors, text colors, status colors
- **Typography** - Font families, sizes, weights, spacing
- **Spacing** - Consistent spacing scale
- **Border Radius** - Corner radius values
- **Shadows** - Elevation and depth
- **Components** - Component-specific tokens
- **Breakpoints** - Responsive design breakpoints

## 🚀 Benefits

✅ **Organized Structure** - Clear file categorization
✅ **Scalable** - Easy to add new components and tokens
✅ **Maintainable** - Logical separation of concerns
✅ **Team-Friendly** - Clear documentation and structure
✅ **CI/CD Ready** - Automated token synchronization

## 📞 Support

For questions or issues:
1. Check the documentation in `/docs/`
2. Review the token structure in `/tokens/`
3. Test scripts with `npm run check-tokens`
# tokendls
