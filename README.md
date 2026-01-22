# Lucrec.io

## Software that Scales

Boutique software development firm specialized in automation, code rescue, and high-performance digital products. Not agencies, engineers.

## About

Lucrec.io is a software development & innovation consultancy that builds real software engineering solutions for companies that understand the true cost of technical debt. We build systems, not just pages.

With a distributed team of 26 engineers across Latin America, USA, Europe, and Asia, we offer near-shore overlap for US clients while leveraging global talent. We turn timezone differences into a productivity advantage.

## Services

### Digital Products & MVPs

Launching your product in weeks, not months. Scalable, atomic architecture from Day 1.

### Automation & AI Agents

We replace manual labor with Python scripts and LLMs. Efficiency is not optional.

### Code Rescue & Refactoring

If your current team says 'we need to rewrite everything', call us first.

## Philosophy

Our approach is inspired by the Roman philosopher Lucretius and grounded in fundamental engineering principles:

- **Digital Atomism**: Complex systems built from simple, indivisible, and robust components.
- **Ex Nihilo Nihil Fit**: Nothing comes from nothing. We optimize resources because we understand server physics.
- **Clarity Over Fear**: We eliminate the fear of 'Technical Debt'. Our code is transparent and auditable.

> *Understanding the nature of your software.*

## Website

This repository contains the source code for the Lucrec.io landing page, built with HTML, CSS (Tailwind), and JavaScript.

### Project Structure

```text
lucrec.io/
├── index.html              # Main HTML file
├── css/                    # Stylesheets
│   ├── style.css          # Main stylesheet
│   ├── vendors/           # Third-party CSS (AOS animations)
│   └── additional-styles/ # Custom component styles
├── js/                    # JavaScript files
│   ├── main.js           # Main JavaScript logic
│   └── vendors/          # Third-party libraries (Alpine.js, AOS)
├── images/                # Image assets
├── fonts/                 # Custom fonts (Uncut Sans)
├── robots.txt            # Search engine crawler instructions
├── sitemap.xml           # XML sitemap for SEO
├── Dockerfile            # Docker configuration
└── docker-compose.yml    # Docker Compose configuration
```

### SEO Features

The website includes comprehensive SEO optimizations:

- **Meta Tags**: Enhanced title, description, keywords, and Open Graph tags
- **Structured Data**: JSON-LD schema markup for ProfessionalService, Organization, and WebSite
- **Social Media**: Optimized Open Graph and Twitter Card tags with images
- **Performance**: Preconnect and DNS-prefetch for faster resource loading
- **Accessibility**: Descriptive alt text for all images
- **Search Engine Files**: `robots.txt` and `sitemap.xml` for better crawlability

### Getting Started

#### Using Docker (Recommended)

The site can be run using Docker with live file synchronization. Changes to local files are immediately reflected in the container.

1. Ensure Docker and Docker Compose are installed

2. Build and start the container:

   ```bash
   docker-compose up -d --build
   ```

3. Access the site at `http://localhost:8080`

4. Stop the container:

   ```bash
   docker-compose down
   ```

The Docker setup uses a volume mount, so all local file changes are immediately available in the container without rebuilding.

#### Manual Setup

1. Ensure Node.js and npm are installed

2. Install dependencies:

   ```bash
   npm install
   ```

3. Build CSS:

   ```bash
   npm run build
   ```

4. For development with auto-rebuild:

   ```bash
   npm run dev
   ```

### Technologies Used

- **HTML5**: Semantic markup with proper structure
- **Tailwind CSS**: Utility-first CSS framework
- **Alpine.js**: Lightweight JavaScript framework for interactivity
- **AOS (Animate On Scroll)**: Scroll animations library
- **Custom Fonts**: Uncut Sans font family

## Contact

- **Email**: [audit@lucrec.io](mailto:audit@lucrec.io)
- **Website**: [https://lucrec.io](https://lucrec.io)

---

© 2026 Lucrec.io. All rights reserved.
