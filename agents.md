# AI Agent Context: nleigh.github.io

## Project Overview
This repository (`nleigh.github.io`) is the personal portfolio and blog website for Nathan Leigh. It is a static website hosted on GitHub Pages, built using HTML, CSS, and JavaScript, and based on a customized Start Bootstrap theme ("Freelancer"). It serves as a showcase for Nathan's professional background as a Cloud Engineer, his CV, his Medium articles on technology, and various web/software projects (e.g., Exponential Disruption, Live Like A Cat, Android Restaurant System).

## Technology Stack
- **Core Languages:** HTML5, CSS3, JavaScript
- **Frameworks & Libraries:** 
  - Bootstrap (v4.x based on the vendor folder structure)
  - jQuery
  - FontAwesome (for icons)
  - Magnific Popup (for portfolio modals)
- **Styling Preprocessor:** SCSS (Sass)
- **CI/CD:** Travis CI (`.travis.yml` present)
- **Hosting:** GitHub Pages (with custom domain indicated by the `CNAME` file)

## Repository Structure
- `index.html`: The main landing page, containing the hero section, portfolio grid, contact information, and CV links.
- `medium-articles.html`, `restaurant-system.html`, `live-like-a-cat.html`: Sub-pages for specific portfolio items.
- `exponential-disruption/`, `live-like-a-cat/`: Directories containing assets and HTML for specific sub-projects.
- `css/`: Compiled CSS files (e.g., `freelancer.min.css`).
- `scss/`: Source SCSS files used to generate the CSS.
- `js/`: Custom JavaScript files (e.g., `freelancer.min.js`, `contact_me.js`).
- `img/`: Image assets used throughout the site.
- `vendor/`: Third-party dependencies (Bootstrap, jQuery, etc.). **Do not modify files in this directory.**

## Agent Instructions & Guidelines

When an AI agent is tasked with modifying or analyzing this repository, it should adhere to the following rules:

### 1. Architectural Consistency
- **Static Site Principles:** Maintain the static nature of the website. Do not introduce server-side logic (e.g., Node.js, Python backends) unless explicitly requested to migrate the architecture.
- **Theme Integrity:** Respect the existing "Freelancer" Bootstrap theme structure. When adding new sections or components, use existing Bootstrap utility classes and grid systems to ensure consistency and responsiveness.

### 2. Styling and CSS/SCSS
- **Use SCSS:** If making significant styling changes, modify the files in the `scss/` directory rather than directly editing the compiled files in the `css/` directory. Note that an external build step may be required to compile SCSS to CSS.
- **Responsive Design:** Ensure all new elements are mobile-friendly and utilize Bootstrap's responsive breakpoints (`col-sm-`, `col-md-`, `col-lg-`).

### 3. File Modifications
- **Vendor Directory:** Treat the `vendor/` directory as read-only. If a dependency needs updating, do it by replacing the directory contents with the new version, rather than editing the minified files directly.
- **HTML Structure:** Keep semantic HTML tags. Ensure any new images have appropriate `alt` tags for accessibility.
- **Navigation:** If adding a new page or a significant section to `index.html`, ensure the navigation bar (`#mainNav`) is updated accordingly so users can access the new content.

### 4. Code Quality
- **Formatting:** Match the existing indentation and formatting style of the HTML, CSS, and JS files.
- **Minification:** If modifying JS or CSS directly (e.g., `freelancer.min.js`), ideally the unminified source should be edited and then minified, or ensure the edits are clean if only the minified file is available. 

### 5. Deployment
- **GitHub Pages:** Be aware that changes pushed to the main branch are automatically deployed via GitHub Pages. Ensure all internal links are relative and will resolve correctly on the live site (`nathanleigh.co.uk` or the respective `.github.io` domain).
