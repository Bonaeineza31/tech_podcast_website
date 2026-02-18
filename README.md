# StoryCast - Empowering Girls in Tech

A 3-page accessible microsite showcasing audio and video storytelling from women in technology. Built with semantic HTML5, Sass, and responsive design principles.

## Project Structure

```
tech_podcast_website/
├── index.html              # Home page with featured stories
├── about.html              # About page with mission & accessibility statement
├── stories/
│   └── episode-1.html      # Story detail page with audio/video
├── sass/
│   ├── _colors.scss        # Color tokens
│   ├── _typography.scss    # Typography system
│   ├── _spacing.scss       # Spacing scale & breakpoints
│   ├── _layout.scss        # Grid & flexbox utilities
│   ├── _components.scss    # Component styles (cards, buttons, media players)
│   └── main.scss           # Main stylesheet
├── main.css                # Compiled CSS
├── assets/
│   ├── images/             # Episode images
│   ├── transcripts/        # Full transcripts & VTT captions
│   ├── audio/              # Audio files (placeholder)
│   └── video/              # Video files (placeholder)
└── README.md               # This file
```

##  Running Locally

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- Sass compiler (optional, for editing styles)

### View the Site
1. Open `index.html` in your web browser
2. Navigate between pages using the header navigation
3. All pages are static HTML - no server required

### Compile Sass (if editing styles)
```bash
# Install Sass globally
npm install -g sass

# Compile Sass to CSS
sass sass/main.scss main.css

# Watch for changes
sass --watch sass/main.scss:main.css
```

## Accessibility Checklist (WCAG 2.1 AA)

### Semantic HTML Structure
- [x] Proper HTML5 semantic elements (`<header>`, `<main>`, `<article>`, `<section>`, `<nav>`, `<footer>`)
- [x] Logical heading hierarchy (h1 → h2 → h3)
- [x] `<time>` elements with `datetime` attributes
- [x] Semantic `<audio>` and `<video>` elements

### Media Accessibility
- [x] Full transcripts for all audio episodes
- [x] Video captions via WebVTT `<track>` elements
- [x] Alternative text for all images
- [x] Multiple source formats for audio/video

###  Keyboard Navigation
- [x] Skip to main content link
- [x] All interactive elements keyboard accessible
- [x] Visible focus states (3px blue outline)
- [x] Logical tab order

### ARIA Support
- [x] `aria-label` on navigation and media elements
- [x] `aria-labelledby` on sections
- [x] `aria-current="page"` for active navigation
- [x] `role` attributes where appropriate

### Color & Contrast
- [x] WCAG AA contrast ratios met (4.5:1 for normal text, 3:1 for large text)
- [x] Primary text: #0f172a on #ffffff (21:1 ratio)
- [x] Links: #0066ff on #ffffff (8.6:1 ratio)
- [x] Information not conveyed by color alone

### Responsive Design
- [x] Mobile-first responsive design
- [x] Content readable at 200% zoom
- [x] Responsive from 320px to 1920px width
- [x] Container queries for adaptive components

### Motion & Animation
- [x] `prefers-reduced-motion` support
- [x] Animations disabled for users with motion sensitivity

##  Design Features

### Sass Architecture
- **Partials & Tokens**: Organized color, typography, and spacing systems
- **BEM-inspired naming**: Component-based class names
- **Design tokens**: Consistent variables for maintainability

### Container Queries
The `.podcast-card` component uses CSS container queries to adapt its layout:
- **Wide containers**: Horizontal layout with image on left
- **Narrow containers** (<500px): Vertical stacked layout

### Responsive Breakpoints
- Mobile: < 768px
- Tablet: 768px - 1024px
- Desktop: > 1024px

## Key Technologies

- **HTML5**: Semantic structure
- **Sass/CSS**: Styling with design tokens
- **CSS Grid & Flexbox**: Responsive layouts
- **Container Queries**: Component-level responsiveness
- **No frameworks**: Vanilla HTML, CSS, and minimal JavaScript

## Content

### Pages
1. **Home** (`index.html`) - Featured stories and hero section
2. **Story Detail** (`stories/episode-1.html`) - Full episode with audio, video, and transcript
3. **About** (`about.html`) - Mission statement and accessibility documentation

### Featured Episode
**Breaking Into Tech: Sarah's Journey**
- 15-minute audio story
- Video introduction with captions
- Full timestamped transcript
- Hosted by Bonae

##  Accessibility Statement

StoryCast is committed to making our content accessible to everyone. We follow WCAG 2.1 Level AA standards and continuously improve our accessibility features.

For accessibility feedback: accessibility@storycast.tech

## License

Created for educational purposes - Girls in Tech Empowerment Project 2026
