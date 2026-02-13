# Portfolio Website Project

## Project Overview

This is a modern, dark-themed portfolio website for **Omair Al-Qahtani**, a Creative Designer & Architect based in Riyadh, Saudi Arabia. The website showcases professional work, experience, and skills with premium animations and smooth interactions.

## Technology Stack

### Core Technologies

- **HTML5** - Semantic markup structure
- **Tailwind CSS v4.1.18** - Utility-first CSS framework
- **Vanilla JavaScript** - No framework dependencies for maximum performance

### Animation & Interaction Libraries

- **Lenis v1.0.42** - Smooth scroll library (Framer-style)
- **Framer Motion v10.16.4** - Advanced animations and scroll-based effects
- **Lucide Icons** - Modern icon library

### Fonts

- **Inter** - Primary body font (weights: 300, 400, 500, 600, 700)
- **Space Grotesk** - Display font for headings (weights: 400, 500, 600, 700)

## Project Structure

```
fahad/
## Project Structure

```

fahad/
├── index.html # Main portfolio landing page
├── al-thumama-aviation-club.html # Detail page: Aviation Club
├── college-architecture-arts.html # Detail page: Architecture College
├── lucid-air.html # Detail page: LucidAir Showroom
├── main.js # Shared logic and animations
├── src/
│ ├── output.css # Compiled Tailwind styles

````

... [rest of standard sections] ...

---

## Recent Changes

### 2026-02-13 - Project Detail Pages Implementation

**Added:**
- ✅ Created 3 individual project detail pages:
  - `al-thumama-aviation-club.html`
  - `college-architecture-arts.html`
  - `lucid-air.html`
- ✅ Implemented premium architectural layout for detail pages:
  - Large hero visuals with dynamic italic headers
  - Detailed design philosophy sections
  - Technical project specification sidebars
  - High-end typography (Space Grotesk + Inter)
  - Next/Previous project navigation for seamless browsing

**Modified:**
- 🔄 `index.html` - Linked project cards to their respective detail pages
- 🔄 `index.html` - Enhanced project cards with better hover states and clickability
- 🔄 Optimized Tailwind classes for better standards compliance (aspect-ratio, background opacity)

**Result:**
The portfolio now offers a deep-dive experience into each architectural work, providing comprehensive details and a more professional presentation of individual projects.

---

### 2026-02-13 - Real Portfolio Projects Integration

### 1. **Framer-Style Smooth Scrolling**

- Implemented using Lenis smooth scroll library
- Buttery-smooth momentum-based scrolling
- Custom easing function: `easeOutExpo`
- Duration: 1.2s for optimal feel

### 2. **Hero Section**

- Fixed position with parallax effect
- Dynamic project preview images that follow mouse movement
- Fade and blur effects on scroll
- Responsive image positioning

### 3. **Scroll-Based Animations**

- Hero content fade and scale on scroll
- Timeline progress indicator in Experience section
- Navbar background blur on scroll
- About text color interpolation
- All animations use Lenis scroll events for smoothness

### 4. **Interactive Elements**

- 3D tilt effect on project cards
- Neon glow button effects
- Animated timeline dots
- Infinite ticker animation for tools/software
- Mobile menu with smooth transitions

### 5. **Performance Optimizations**

- Lazy loading for images
- RequestAnimationFrame for smooth animations
- Passive scroll listeners
- Reduced motion support for accessibility
- Optimized asset loading

## Sections

1. **Hero** - Full-screen introduction with animated background images
2. **About Me** - Personal introduction with contact information
3. **Work Experience** - Timeline-based experience showcase
4. **Tools & Software** - Infinite scrolling ticker of design tools
5. **Selected Works** - Grid of portfolio projects
6. **Footer/Contact** - Contact information and social links

## Design System

### Color Palette

- **Background Primary**: `#0f0f0f` (Deep black)
- **Background Secondary**: `#000f26` (Dark blue)
- **Text Primary**: `#ffffff` (White)
- **Text Secondary**: `rgba(255, 255, 255, 0.6)` (60% white)
- **Text Muted**: `rgba(255, 255, 255, 0.4)` (40% white)

### Effects

- **Neon Glow**: Subtle blue glow on interactive elements
- **Blur Effects**: Backdrop blur for navbar and overlays
- **Transitions**: Cubic-bezier easing for smooth feel

## Browser Support

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Responsive design for mobile, tablet, and desktop
- Graceful degradation for older browsers
- Accessibility features (ARIA labels, semantic HTML)

## Development

### Build Commands

```bash
# Watch mode for development
npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch

# Production build (minified)
npx tailwindcss -i ./src/input.css -o ./src/output.css --minify
````

### Local Development

Simply open `index.html` in a modern web browser. No build server required for basic development.

## Accessibility Features

- Semantic HTML5 elements
- ARIA labels and roles
- Keyboard navigation support
- Reduced motion support via `prefers-reduced-motion`
- High contrast mode support
- Screen reader friendly

## Performance Metrics

- **Smooth Scrolling**: 60 FPS maintained
- **Animation Performance**: Hardware-accelerated transforms
- **Load Time**: Optimized with lazy loading
- **Bundle Size**: Minimal dependencies, CDN-based libraries

---

## Recent Changes

### 2026-02-13 - Real Portfolio Projects Integration

**Replaced:**

- 🔄 Removed 4 dummy placeholder projects with Unsplash images
- ✅ Added 3 real portfolio projects with local images

**Projects Added:**

1. **Al Thumama Aviation Club** (University Project)
   - Image: `src/projects/Al Thumama Aviation Club.png`
   - Description: Aviation club design with modern facilities and training spaces
2. **College of Architecture and Arts** (University Project)
   - Image: `src/projects/College of Architecture and Arts.png`
   - Description: Educational campus design with flexible learning spaces
3. **LucidAir** (Personal Project)
   - Image: `src/projects/LucidAir.png`
   - Description: Luxury automotive showroom concept

**Modified:**

- 🔄 `index.html` - Portfolio section (lines 503-567)
  - Updated project cards with real titles, descriptions, and images
  - Reduced from 4 to 3 projects to match available content
- 🔄 `index.html` - Hero section (lines 91-115)
  - Replaced 5 Unsplash preview images with 3 real project images
  - Updated hero background animations to cycle through actual projects

**Result:**
The portfolio now showcases authentic work with high-quality project images and accurate descriptions.

---

### 2026-02-13 - Framer-Style Smooth Scrolling Implementation

**Added:**

- ✅ Lenis smooth scroll library (v1.0.42) via CDN
- ✅ `initLenisScroll()` function with optimal configuration
  - Duration: 1.2s
  - Easing: easeOutExpo curve
  - Mouse multiplier: 1
  - Touch multiplier: 2
- ✅ Integrated Lenis with all scroll-based animations:
  - Hero section fade/blur effects
  - Timeline progress animation
  - Navbar background transitions
  - About text color interpolation
  - Smooth anchor link scrolling

**Modified:**

- 🔄 `initHeroAnimations()` - Now uses Lenis scroll events
- 🔄 `initTimelineAnimation()` - Integrated with Lenis
- 🔄 `initSmoothScroll()` - Uses `lenis.scrollTo()` for anchor links
- 🔄 `initNavbarScroll()` - Lenis-based scroll detection
- 🔄 `initAboutTextAnimation()` - Lenis scroll events
- 🔄 `src/input.css` - Added Lenis CSS classes and disabled native smooth scroll

**Performance Improvements:**

- ⚡ Removed redundant `requestAnimationFrame` throttling (Lenis handles this)
- ⚡ Eliminated multiple scroll event listeners in favor of single Lenis instance
- ⚡ Smoother 60 FPS scrolling experience

**Technical Details:**

- All scroll handlers now accept `lenis` parameter
- Fallback to native scroll if Lenis fails to load
- Scroll position accessed via `lenis.scroll` instead of `window.scrollY`
- Custom easing function: `(t) => Math.min(1, 1.001 - Math.pow(2, -10 * t))`

**Result:**
The website now has buttery-smooth, Framer-style scrolling throughout all sections with optimized performance and consistent animation timing.

---

## Future Enhancements

- [ ] Add more portfolio projects
- [ ] Implement project detail pages
- [ ] Add blog section
- [ ] Integrate contact form with backend
- [ ] Add dark/light mode toggle
- [ ] Implement i18n for Arabic language support
- [ ] Add loading animations
- [ ] Optimize images with WebP format
- [ ] Add service worker for offline support

## Contact Information

**Omair Al-Qahtani**

- Email: Omairalrooq@outlook.com
- Phone: +966 532 101 058
- Location: Riyadh, Saudi Arabia
- LinkedIn: [Omair Al-Qahtani](https://linkedin.com)

---

_Last Updated: February 13, 2026_
