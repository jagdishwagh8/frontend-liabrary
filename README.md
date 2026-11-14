# WEBLYTIC — Frontend Component Library

A curated collection of reusable, responsive website sections built
with pure HTML, CSS and JavaScript. Browse ready-made navigation
bars, hero sections, about blocks, galleries, services, contact
forms and footers — then copy the code straight into your own
project.

No frameworks. No build step. No dependencies.

Live Demo: https://jwagh8237.github.io/weblytic/


------------------------------------------------------------------------
HIGHLIGHTS
------------------------------------------------------------------------

- 4 distinct design styles: Minimal, Luxury, Professional, Versatile
- 7+ section categories per style: Navbar, Hero, About, Gallery,
  Services, Contact, Footer
- One-click "Copy" button on every code block
- Zero dependencies — pure HTML, CSS and vanilla JavaScript
- Fully responsive — tested from 360px mobile to ultra-wide desktop
- Accessibility-minded — semantic markup, focus-visible styles,
  prefers-reduced-motion support
- Isolated components — scoped CSS so sections never clash
- CSS custom properties for easy re-theming


------------------------------------------------------------------------
DESIGN STYLES
------------------------------------------------------------------------

MINIMAL       → minimal.html
                Clean typography, generous white space, restrained
                monochrome palette.

LUXURY        → luxury.html
                Editorial serif type, warm neutrals, gold accents,
                generous imagery.

PROFESSIONAL  → professional.html
                Corporate navy and blue, structured grids,
                trust-first layout.

VERSATILE     → versatile.html
                Glassmorphism, gradient backgrounds, dark UI with
                high contrast.

Each style page follows the same navigation structure so you can
compare layouts side by side.


------------------------------------------------------------------------
AVAILABLE SECTIONS
------------------------------------------------------------------------

NAVBAR
  - Centered link
  - Right link
  - Transparent / overlay

HERO
  - Centered
  - Split layout
  - Background image

ABOUT
  - Timeline
  - Values / story
  - Split layout

GALLERY
  - Featured
  - Grid
  - Cards

SERVICES
  - Icon grid
  - 3-column cards
  - 3x2 image cards

CONTACT
  - Info / form
  - Map + form
  - Centered form

FOOTER
  - Compact
  - Full


------------------------------------------------------------------------
TECH STACK
------------------------------------------------------------------------

HTML5        Semantic, accessible markup
CSS3         Custom properties, grid, flexbox, clamp(),
             glassmorphism, backdrop-filter
JavaScript   Vanilla only — copy-to-clipboard, mobile menu toggle,
             interactive featured gallery
No framework No React, Vue, Tailwind, Bootstrap or jQuery


------------------------------------------------------------------------
PROJECT STRUCTURE
------------------------------------------------------------------------

weblytic/
  index.html            Landing page — style chooser
  minimal.html          Minimal style library
  luxury.html           Luxury style library
  professional.html     Professional style library
  versatile.html        Versatile style library

  logo.png              Site logo
  favicon.png           Browser favicon
  og-image.jpg          Social share image

  images/
    minimal.webp        Landing card previews
    luxury.webp
    professional.webp
    versatile.jpg
    1.png ... 120.png   Section previews

Section styles are fully inlined inside each *.html file (inside
<style> and <pre> blocks), so you can copy a single section and it
just works.


------------------------------------------------------------------------
GETTING STARTED
------------------------------------------------------------------------

1. Clone the repository

   git clone https://github.com/jwagh8237/weblytic.git
   cd weblytic

2. Serve it locally

   Everything is static, so no server is strictly required — but
   for the copy-to-clipboard button to work (navigator.clipboard),
   serve the files over localhost or HTTPS.

   Python:
       python -m http.server 8000

   Node:
       npx serve .

   VS Code:
       Use the "Live Server" extension.

   Then open: http://localhost:8000/

3. Use a component

   - Open any style page (e.g. minimal.html).
   - Find the section you want.
   - Click "Copy" on the code block.
   - Paste the <section> + <style> into your project.
   - Re-theme via the CSS custom properties at the top of the
     component (e.g. --hero-bg, --msc-accent).


------------------------------------------------------------------------
CUSTOMISING COMPONENTS
------------------------------------------------------------------------

Every component uses scoped CSS custom properties, so you can
re-theme without touching the stylesheet.

Example — retheme the Minimal About section:

    .mr-about {
      --mr-ink:    #243447;
      --mr-muted:  #687584;
      --mr-accent: #aa8b5e;    /* accent colour */
      --mr-bg:     #faf9f6;
    }

- Colours  → change the custom properties
- Fonts    → replace the font-family declarations
- Spacing  → adjust padding / gap / clamp() values
- Images   → swap the src URLs (Unsplash placeholders work by default)


------------------------------------------------------------------------
ACCESSIBILITY AND PERFORMANCE
------------------------------------------------------------------------

Every component is built with:

- Semantic HTML (<section>, <header>, <footer>, <nav>, <article>)
- aria-label, aria-hidden, aria-pressed, and role where appropriate
- Visible :focus-visible outlines
- @media (prefers-reduced-motion: reduce) blocks that disable
  animation and transition
- Responsive breakpoints at 900px, 768px, 600px, 480px and 380px
  (depending on the component)
- Lazy-loaded images where safe (loading="lazy")
- fetchpriority="high" on hero images


------------------------------------------------------------------------
BROWSER SUPPORT
------------------------------------------------------------------------

Latest two versions of:

  Chrome   Yes
  Firefox  Yes
  Safari   Yes
  Edge     Yes

Older browsers may lack backdrop-filter (glass effect) or :has().
Components still function, just with simplified visuals.


------------------------------------------------------------------------
CONTRIBUTING
------------------------------------------------------------------------

Contributions are welcome.

1. Fork the repo
2. Create a branch: git checkout -b feature/new-section
3. Add your component in the correct *.html file (or a new file,
   if it's a new style)
4. Follow the existing structure:
   image preview → code block → copy button
5. Test responsively at 360px, 768px, 1024px and 1440px
6. Open a Pull Request with a screenshot of the new component

Guidelines:

- Keep components dependency-free
- Use CSS custom properties for theming
- Scope all CSS to the component's root class
- Include prefers-reduced-motion handling
- Include :focus-visible states for interactive elements
- Use meaningful aria-* attributes


------------------------------------------------------------------------
ROADMAP
------------------------------------------------------------------------

[ ] Pricing section category
[ ] Testimonials section category
[ ] FAQ section category
[ ] Blog / Article layouts
[ ] Dark mode toggle per style
[ ] Export components as standalone .html files
[ ] Optional Tailwind CSS variants


------------------------------------------------------------------------
AUTHOR
------------------------------------------------------------------------

Jagdish Wagh
GitHub: https://github.com/jwagh8237


------------------------------------------------------------------------
LICENSE
------------------------------------------------------------------------

MIT License.

You are free to use, modify and distribute the components in
personal and commercial projects. Attribution is appreciated but
not required.


------------------------------------------------------------------------
CREDITS
------------------------------------------------------------------------

- Placeholder imagery: Unsplash (https://unsplash.com/)
- Icons: hand-crafted inline SVG (no icon library dependency)
- Typography fallbacks: system UI stack + Georgia serif for
  editorial styles


------------------------------------------------------------------------
SUPPORT
------------------------------------------------------------------------

If WEBLYTIC saved you time, consider giving the repo a star — it
helps others find the library and keeps development going.

Found a bug?       https://github.com/jwagh8237/weblytic/issues
Have a suggestion? https://github.com/jwagh8237/weblytic/discussions


------------------------------------------------------------------------

Built with care, one section at a time.
WEBLYTIC — Versatile Frontend Component Library
