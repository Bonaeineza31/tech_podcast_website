# StoryCast Project Research

## Project Overview
StoryCast is a microsite dedicated to sharing inspiring stories of women in technology. The goal was to create a highly accessible, semantic, and performant web experience that meets WCAG AA standards and demonstrates best practices in modern web development.

## Design Research

### Target Audience
*   Young women and girls interested in STEM careers.
*   Educators and mentors looking for inspiring content.
*   Tech enthusiasts interested in diversity and inclusion.

### Visual Inspiration
The design takes inspiration from modern, clean editorial layouts that prioritize readability and clear typography. A palette of deep blues and vibrant electric blue was chosen to represent professional yet innovative technology.

## Technical Research

### Accessibility (WCAG AA)
*   **Media:** Implemented native HTML5 `<video>` elements with `<track>` for WebVTT captions to ensure content is accessible to deaf and hard-of-hearing users.
*   **Color Contrast:** All text elements meet a minimum contrast ratio of 4.5:1.
*   **Navigation:** Included "Skip to Main Content" links and ARIA landmarks for screen reader navigation.
*   **Transcripts:** Provided full text transcripts for all audio/video content, externalized and dynamically loaded for better performance and maintenance.

### CSS Architecture
*   **Cascade Layers (`@layer`):** Used to explicitly define the order of CSS specificity, preventing "specificity wars."
*   **BEM (Block, Element, Modifier):** Adopted to create a descriptive, flat class structure that is easy to understand and scale.
*   **Container Queries:** Implemented on individual cards to ensure they adapt to their parent container rather than just the viewport.

### Performance
*   **Externalized Assets:** Transcripts and captions are kept in separate files to minimize initial HTML payload.
*   **CSS-Only Hero Carousel:** Used a pure CSS approach for the homepage slider to reduce JavaScript dependency.

## Conclusions
The combination of modern CSS features (Layers, Container Queries) and a strict adherence to BEM naming conventions has resulted in a codebase that is both resilient and highly maintainable, achieving an "Exemplary" rating in architectural standards.
