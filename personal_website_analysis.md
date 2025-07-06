# Personal Website Analysis: Hugo Themes Comparison

This document analyzes personal websites built with three popular Hugo themes: Blowfish, PaperMod, and Hugo Academic/Blox. Each theme offers distinct features and design philosophies suitable for different use cases.

## Blowfish Theme Examples

### 1. nunocoracao.com (n9o.xyz)
**Owner:** Nuno Coração (Principal Product Manager @ Docker)
**Role:** Creator of the Blowfish theme

#### Key Features:
- Creator of the Blowfish theme itself
- Demonstrates all theme capabilities
- Clean, modern design with Tailwind CSS
- Multiple color schemes including Neon
- Dark mode with auto-switching
- Background layout options

#### Strengths:
- Comprehensive documentation
- Active development and community support (600+ GitHub stars)
- CLI tool for easy setup
- Highly customizable with configuration files
- Responsive design optimized for all devices

#### Technical Implementation:
- Built with Tailwind CSS 3.0
- Supports multiple installation methods (git submodule, Hugo Module, manual)
- Automatic image optimization
- Built-in site search functionality

### 2. mertbakir.gitlab.io
**Owner:** Mert Bakır
**Focus:** Coding, static sites, algorithms, mathematical problems, R, and Python

#### Key Features:
- Custom-built theme from scratch (not actually using Blowfish)
- Focus on technical content and tutorials
- Clean, minimalist design
- Hugo-specific tutorials and guides

#### Strengths:
- Extensive Hugo documentation and tutorials
- Clean code examples
- Well-organized content structure
- Version history tracking

#### Unique Elements:
- Custom SCSS implementation
- Hugo debugging techniques shared
- Migrated from Jekyll to Hugo

### 3. paigepierce.dev
*Note: Limited information available from searches*

### 4. dr460nf1r3.org
*Note: Limited information available from searches*

### 5. omarohn.de
*Note: Limited information available from searches*

## PaperMod Theme Examples

### 1. jessewei.dev
**Owner:** Jesse Wei
**Status:** Migrated from PaperMod to Jekyll/al-folio

#### Key Features:
- Previously used PaperMod with extensive modifications
- Maintained diff documentation showing customizations
- Deployed on Netlify
- Clean, minimalist design

#### Strengths:
- Well-documented migration process
- Open-source modifications available on GitHub
- Good example of theme customization

#### Weaknesses Identified:
- Missing necessary functionality in PaperMod
- Required extensive modifications
- Eventually migrated away due to limitations

### 2. rubendibattista.github.io
*Note: Limited specific information available*

### 3. arkalim.github.io (notes.arkalim.org)
**Owner:** Abdur
**Focus:** Technical notes and documentation

#### Key Features:
- Uses PaperMod theme
- Focus on static site generators
- Technical documentation repository

#### PaperMod Features Demonstrated:
- Regular, Home-Info, and Profile modes
- Table of Contents generation
- Archive functionality
- Cover images with responsive support
- Code block copy buttons
- Chroma syntax highlighting
- Fuse.js search integration
- Social media integration
- Multilingual support
- Light/Dark theme switching

### 4. sudhir-j-d.github.io
*Note: Limited specific information available*

## Hugo Academic/Blox Examples

### 1. mickaellalande.github.io
**Owner:** Mickaël Lalande
**Focus:** Academic content with comprehensive tutorials

#### Key Features:
- Detailed tutorial on setting up Academic/Wowchemy/Hugo Blox
- Acknowledges frequent theme name changes
- GitHub Pages deployment focus
- Academic-oriented design

#### Strengths:
- Excellent documentation for beginners
- Step-by-step setup guides
- Troubleshooting tips included
- Active maintenance

#### Technical Details:
- Uses academic-kickstart repository structure
- Automatic GitHub Pages deployment
- Snap installation recommended for Linux

### 2. matteocourthoud.github.io
**Owner:** Matteo Courthoud
**Background:** PhD in Economics, University of Zürich

#### Key Features:
- Custom Wowchemy theme modifications
- Comprehensive setup tutorial published
- GitHub repository with custom settings
- Focus on economics and data science

#### Strengths:
- Open-source custom theme available
- Detailed implementation guide
- Google Search Console integration
- Knowledge sharing philosophy

#### Unique Elements:
- Custom theme repository (matteocourthoud/custom-wowchemy-theme)
- Blogdown and Hugo integration
- Advanced customization examples

### 3. hrishikeshrt.github.io
**Owner:** Hrishikesh Terdalkar
**Focus:** Computational Linguistics, NLP, Sanskrit

#### Key Features:
- Detailed setup tutorial for GitHub Pages
- Focus on low-resource languages
- Academic portfolio showcase
- Research-oriented design

#### Strengths:
- Clear deployment instructions
- Submodule-based deployment strategy
- Academic CV integration
- Multi-language support

#### Technical Implementation:
- GitHub Pages deployment with submodules
- Static site generation in public/ directory
- Hugo Academic CLI for BibTeX import

### 4. nicolepaul.io
**Owner:** Nicole Paul
**Deployment:** Netlify with Cloudflare domain management

#### Key Features:
- Text editor-based maintenance
- Custom CSS styling (assets/scss/custom.scss)
- Markdown-based content management
- Automatic deployment via Netlify

#### Strengths:
- Cost-effective ($45/year for domain only)
- Fast deployment (1-2 minutes)
- High degree of control
- Clean, professional design

#### Technical Details:
- Content in markdown files within content/ folder
- Landing page at content/_index.md
- Custom styling overrides default theme
- No JavaScript/HTML knowledge required

## Summary of Findings

### Blowfish Theme
**Best for:** Modern personal websites with emphasis on visual design
- Pros: Active development, extensive customization, modern tech stack
- Cons: Relatively new, may have breaking changes

### PaperMod Theme
**Best for:** Minimalist blogs and documentation sites
- Pros: Clean design, fast performance, good feature set
- Cons: May require modifications for advanced features

### Hugo Academic/Blox
**Best for:** Academic portfolios and research showcases
- Pros: Purpose-built for academics, publication management, professional layouts
- Cons: Frequent rebranding, can be complex for beginners

## Common Strengths Across All Themes:
1. Static site generation for fast performance
2. GitHub Pages/Netlify deployment options
3. Markdown-based content management
4. Responsive design
5. SEO optimization
6. Dark mode support

## Common Weaknesses:
1. Learning curve for Hugo beginners
2. Theme-specific customization limitations
3. Documentation can become outdated
4. Migration between themes can be complex