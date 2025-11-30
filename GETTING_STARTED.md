# Getting Started with Your Swiss Design Gallery

## Prerequisites Installation

Since Node.js is not currently installed on your system, you'll need to install it first.

### Install Node.js and npm

```bash
# Install Node.js and npm
sudo apt update
sudo apt install nodejs npm -y

# Verify installation
node --version  # Should show v12.x or higher
npm --version   # Should show 6.x or higher
```

Alternatively, for the latest LTS version:

```bash
# Using NodeSource repository for Node.js 20.x
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
sudo apt-get install -y nodejs
```

## Running the Project

Once Node.js is installed:

```bash
# Navigate to project directory
cd /home/isalora101/ial23-blip.github.io

# Install dependencies
npm install

# Start development server
npm run dev
```

The site will be available at: `http://localhost:8080`

## Building for Production

```bash
# Build the site
npm run build

# Output will be in _site/ directory
```

## Project Commands

- `npm run dev` - Start development server with live reload
- `npm run build` - Build site for production
- `npm run clean` - Remove build directory

## Next Steps

1. **Install Node.js** using the commands above
2. **Run `npm install`** to install Eleventy and dependencies
3. **Run `npm run dev`** to start the development server
4. **Open browser** to `http://localhost:8080` to view your site
5. **Make changes** - the site will automatically reload
6. **Commit to GitHub** - automatic deployment will handle the rest

## GitHub Pages Setup

To enable automatic deployment:

1. Go to your repository settings on GitHub
2. Navigate to **Pages** section
3. Under "Build and deployment", select **GitHub Actions**
4. Push your code to the `main` branch
5. GitHub Actions will automatically build and deploy your site

Your site will be live at: `https://ial23-blip.github.io`

## Troubleshooting

### Port 8080 already in use
```bash
# Use a different port
npx eleventy --serve --port=3000
```

### Build errors
```bash
# Clear cache and reinstall
rm -rf node_modules package-lock.json
npm install
```

### Can't find module errors
```bash
# Make sure all dependencies are installed
npm install
```

## File Structure Summary

Your project now includes:

- **5 complete pages**: Home, History, Principles, Examples, About
- **Complete CSS design system**: Variables, reset, base, layout, components
- **Responsive layouts**: Grid systems with mobile breakpoints
- **JavaScript functionality**: Smooth scrolling, animations, navigation
- **Eleventy configuration**: Template engine, data management, build process
- **GitHub Actions workflow**: Automatic deployment to GitHub Pages
- **Comprehensive README**: Project documentation

All pages demonstrate Swiss Design principles through their design and contain substantial content about the design movement's history, key figures, and influence on modern design.

## Making Changes

### Edit Content
- Modify files in `src/` directory
- Pages are in `src/index.njk`, `src/history/index.njk`, etc.
- Site configuration in `src/_data/site.json`

### Update Styles
- CSS files are in `src/css/` directory
- Edit `variables.css` to change colors, spacing, typography
- Component styles in `components.css`

### Add New Pages
```bash
# Create a new page
mkdir src/newpage
nano src/newpage/index.njk
```

Add frontmatter and content, then add link to navigation in `src/_includes/base.njk`

Happy building! 🎨
