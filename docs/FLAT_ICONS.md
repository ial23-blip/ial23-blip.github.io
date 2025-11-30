# Flat Design Icons

## Icon System Overview

All icons follow authentic Flat Design principles:
- **2px stroke weight** - consistent thin outlines
- **Outline style** - no fills (except decorative dots)
- **Minimal detail** - essential shapes only
- **Rounded corners** - stroke-linecap: round, stroke-linejoin: round
- **Monochrome** - single color per icon
- **48x48px base** - scalable with CSS classes
- **Geometric shapes** - circles, rectangles, lines
- **No depth effects** - completely flat

## Icon Sizes

```css
.icon       /* 20x20px - default, navigation */
.icon-lg    /* 48x48px - feature cards, decorative */
.icon-sm    /* 16x16px - inline text */
```

## Icon Colors

```css
.icon-primary   /* Blue #3498DB */
.icon-success   /* Green #2ECC71 */
.icon-warning   /* Orange #F39C12 */
.icon-danger    /* Red #E74C3C */
.icon-white     /* White (for colored backgrounds) */
.icon-dark      /* Dark gray #34495E */
```

## Icon Inventory

### Navigation Icons (20px)
1. **Home** - House outline with door
   - Location: Main navigation, homepage link
   
2. **History** - Clock/time outline
   - Location: History page navigation
   
3. **Principles** - Grid/layout outline
   - Location: Principles page navigation
   
4. **Examples** - Image/gallery outline
   - Location: Examples page navigation
   
5. **About** - Info circle outline
   - Location: About page navigation

### Social/External Icons (20px)
6. **GitHub** - GitHub logo outline
   - Location: Footer connect section
   
7. **External Link** - Arrow out of box
   - Location: External references (when needed)

### Action Icons (20px)
8. **Arrow Right** - Directional arrow
   - Location: CTA buttons, links
   
9. **Download** - Down arrow to line
   - Location: Download actions (when needed)

### Feature Icons (48px)
10. **Layers** - Stacked rectangles (no depth)
    - Location: Homepage "No Depth Effects" card
    - Color: Primary blue
    
11. **Palette** - Color circle with dots
    - Location: Homepage "Vibrant Colors" card
    - Color: Success green
    
12. **Typography** - "T" letterform
    - Location: Homepage "Simple Typography" card
    - Color: Warning orange

### Principle Icons (48px, decorative watermarks)
13. **Minimal Plus** - Rectangle with cross
    - Location: Principles page "Minimal Interface"
    - Opacity: 0.2 (subtle background)
    
14. **Check/Success** - Checkmark
    - Location: Principles page "Digital Honesty"
    - Opacity: 0.2 (subtle background)

### Utility Icons (Available in icons.svg)
15. **Menu/Hamburger** - Three horizontal lines
16. **Star** - Star outline
17. **Book** - Book/documentation outline
18. **Calendar** - Calendar outline
19. **Settings** - Gear outline

## Implementation

### In HTML/Nunjucks:
```html
<!-- Inline SVG with icon classes -->
<svg class="icon icon-primary" viewBox="0 0 48 48" xmlns="http://www.w3.org/2000/svg">
  <circle cx="24" cy="24" r="16"/>
  <path d="M24 12V24L32 28"/>
</svg>
```

### In Navigation:
```html
<a href="/history/">
  <svg class="icon icon-white" viewBox="0 0 48 48">
    <circle cx="24" cy="24" r="16"/>
    <path d="M24 12V24L32 28"/>
  </svg>
  History
</a>
```

### In Buttons:
```html
<a href="/examples/" class="btn btn-primary">
  <svg class="icon icon-white" viewBox="0 0 48 48">
    <rect x="8" y="8" width="32" height="32" rx="2"/>
  </svg>
  View Examples
</a>
```

## Design Rationale

### Why Outline Icons?
- **Flat Design authenticity** - no fills = no depth perception
- **Lighter visual weight** - doesn't overwhelm flat UI
- **Scalability** - strokes scale better than complex shapes
- **iOS 7 heritage** - matches Apple's Flat Design aesthetic

### Why 2px Stroke?
- **iOS 7 standard** - Apple used thin strokes in iOS 7
- **Modern aesthetic** - clean, refined appearance
- **Readability** - visible but not heavy
- **Consistency** - uniform weight across all icons

### Why Minimal Detail?
- **Flat Design principle** - simplicity over complexity
- **Fast recognition** - essential shapes read quickly
- **Scalability** - details lost at small sizes
- **Digital honesty** - no attempt at realism

## Color Usage Guidelines

### Navigation (Header/Footer)
- Always use `icon-white` on colored backgrounds
- Maintains contrast and readability

### Feature Cards
- Use color-matched icons (primary, success, warning)
- Icon color matches card title color

### Principle Pages
- Use `icon-white` on colored principle cards
- Low opacity (0.2) for decorative watermarks

### Buttons
- Match button color scheme
- `icon-white` on colored buttons
- `icon-primary` on white/neutral buttons

## File Locations

- **Icon CSS**: `src/css/icons.css`
- **Icon SVG Library**: `src/images/icons.svg`
- **Compiled CSS**: `_site/css/icons.css`

## References

- iOS 7 Icon Guidelines (2013)
- Flat Icon Design System
- Metro Design Language Icons
- Phosphor Icons (outline style inspiration)
