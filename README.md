# Flat Design Gallery

A comprehensive design gallery exploring Flat Design - the bold, colorful, two-dimensional aesthetic that revolutionized digital interfaces in the 2010s. Created for IS 117: Intro to Website Development.

## 🎨 About

This website documents the history, principles, and influence of Flat Design, from Microsoft's Metro to Apple's iOS 7 and beyond. The site itself is designed using Flat Design principles with vibrant colors, no depth effects, and clean typography.

### Key Topics Covered

- **History**: Origins in Metro design, iOS 7 revolution, evolution to Flat 2.0
- **Principles**: No depth effects, vibrant colors, simple typography, minimal UI
- **Examples**: Windows Phone, iOS 7, modern web applications

## 🚀 Getting Started

### Prerequisites

- Node.js 20.x or higher
- npm

### Installation

```bash
# Clone the repository
git clone https://github.com/ial23-blip/ial23-blip.github.io.git
cd ial23-blip.github.io

# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```

The development server will start at `http://localhost:8080`

## 📁 Project Structure

```
ial23-blip.github.io/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions deployment
├── src/
│   ├── _data/
│   │   └── site.json           # Site configuration
│   ├── _includes/
│   │   └── base.njk            # Base layout template
│   ├── css/
│   │   ├── variables.css       # Design system variables
│   │   ├── reset.css           # CSS reset
│   │   ├── base.css            # Base styles
│   │   ├── layout.css          # Layout components
│   │   └── components.css      # UI components
│   ├── js/
│   │   └── main.js             # JavaScript functionality
│   ├── about/
│   │   └── index.njk           # About page
│   ├── examples/
│   │   └── index.njk           # Examples page
│   ├── history/
│   │   └── index.njk           # History page
│   ├── principles/
│   │   └── index.njk           # Principles page
│   └── index.njk               # Homepage
├── .eleventy.js                # Eleventy configuration
├── .gitignore
├── package.json
└── README.md
```

## 🎨 Design System

The site implements Flat Design principles:

### Typography
- **Font**: Open Sans (fallback to Segoe UI, Tahoma, sans-serif)
- **Scale**: 12px to 56px with bold weights
- **Weights**: 300, 400, 600, 700, 800

### Colors (Flat UI Colors Palette)
- **Primary**: #3498DB (Bright Blue)
- **Success**: #2ECC71 (Green)
- **Warning**: #F39C12 (Orange)
- **Danger**: #E74C3C (Red)
- **Info**: #9B59B6 (Purple)
- **Neutral**: #ECF0F1 (Light Gray)
- **Dark**: #34495E (Dark Gray)

### Design Principles Applied
- Completely flat (no shadows, gradients, or depth)
- Bright, vibrant color palette
- Simple rectangular cards (4px border-radius)
- Bold typography with clear hierarchy
- Line icons (2px stroke)
- Clean, minimal interface elements

## 🛠️ Technology Stack

- **[Eleventy](https://www.11ty.dev/)** - Static site generator
- **[Nunjucks](https://mozilla.github.io/nunjucks/)** - Templating engine
- **CSS Custom Properties** - Design system variables
- **GitHub Actions** - Automated deployment
- **GitHub Pages** - Hosting

## 📦 Deployment

The site automatically deploys to GitHub Pages when changes are pushed to the `main` branch.

### Manual Deployment

```bash
# Build the site
npm run build

# The output is in the _site directory
# Deploy _site contents to your hosting provider
```

## 📚 Learning Outcomes

This project demonstrates:

1. **Design History** - Understanding Flat Design's origins and iOS 7 revolution
2. **Design Principles** - Applying no-depth, colorful, two-dimensional aesthetics
3. **Web Development** - Building modern static sites with Eleventy
4. **Design Systems** - Creating vibrant, maintainable CSS architecture
5. **Version Control** - Using Git and GitHub for project management
6. **CI/CD** - Automated building and deployment with GitHub Actions

## 🤝 Course Information

- **Course**: IS 117 - Intro to Website Development
- **Project**: Swiss Design Lineage Vibe Coding (Flat Design variant)
- **Institution**: New Jersey Institute of Technology
- **Instructor**: Professor Keith Williams

## 📄 License

This project is created for educational purposes as part of IS 117.

## 🙏 Acknowledgments

- Microsoft Metro Team - Pioneering flat design with Windows Phone
- Jony Ive - iOS 7 flat design revolution
- Designmodo - Flat UI toolkit and color palette
- Flat design community - Dribbble, Behance designers
- Professor Keith Williams - Course instruction and project structure

## 🔗 Links

- **Live Site**: [https://ial23-blip.github.io](https://ial23-blip.github.io)
- **Repository**: [https://github.com/ial23-blip/ial23-blip.github.io](https://github.com/ial23-blip/ial23-blip.github.io)
- **Course Repository**: [Swiss Design Lineage Vibe Coding](https://github.com/kaw393939/swiss_design_lineage_vibecoding)

---

Built with Flat Design principles - Clean, Colorful, Two-Dimensional 🎨