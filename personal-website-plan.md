# Job-Market-Ready Personal Website Plan

## Overview
This document outlines a comprehensive plan to transform the current Hugo-based website into an impressive, job-market-ready personal website that showcases technical skills, academic achievements, and professional experience.

## Current State Analysis

### What You Have:
- **Hugo Book theme** installed with basic configuration
- **Content structure** with:
  - `/docs` - Basic introduction page
  - `/til` - "Today I Learned" section (like micro-blogging)
  - `/posts` - Empty blog section
- **Available shortcodes**: buttons, hints, columns, details, tabs, katex, mermaid, sidenote
- **Basic site configuration** with title "One Layer Deeper"

### What's Missing for a Job-Market-Ready Site:
- Professional homepage/landing page
- Comprehensive About section
- CV/Resume page with download functionality
- Project portfolio showcase
- Publications and research section
- Enhanced blog structure
- Professional contact information
- Visual polish and branding

## Key Sections Needed

### 1. **Homepage/About Section**
- Professional summary highlighting both tech skills and academic background
- Clear value proposition
- Professional photo
- Quick links to key sections (CV, Projects, Publications)

### 2. **CV/Resume Section**
- Downloadable PDF version
- Web-friendly version with sections for:
  - Education
  - Work Experience
  - Technical Skills (languages, frameworks, tools)
  - Academic Achievements
  - Certifications

### 3. **Projects/Portfolio Section**
- 3-5 high-quality projects with:
  - Problem statement
  - Solution approach
  - Technologies used
  - Live demos/GitHub links
  - Screenshots/visuals
  - Results/impact

### 4. **Publications/Research Section**
- Peer-reviewed papers
- Conference presentations
- Technical blog posts
- Paper reviews and commentary
- Funny paper screenshots gallery
- Links to full papers (PDFs, arXiv, etc.)
- Citation information

### 5. **Teaching/Mentoring Section** (if applicable)
- Courses taught
- Teaching philosophy
- Student testimonials
- Course materials/resources

### 6. **Blog Enhancement**
- Technical tutorials and deep dives
- Research insights
- Industry observations
- Thought leadership pieces

### 7. **TIL/Zettels Section**
- Short-form content for "working with garage door open"
- Quick insights and learnings
- Technical notes
- Research observations

### 8. **Contact/Connect Section**
- Professional email
- LinkedIn profile
- GitHub profile
- ORCID/Google Scholar (for academics)
- Contact form

## Implementation Phases

### Phase 1: Site Structure & Navigation
1. Create homepage with professional introduction
2. Set up main navigation menu
3. Create section pages (About, CV, Projects, Publications, Blog, Contact)
4. Configure Hugo Book theme settings for better navigation

### Phase 2: Content Development
1. Write compelling About section
2. Create detailed CV page
3. Document 3-5 best projects
4. List publications with proper formatting
5. Write 2-3 initial blog posts
6. Set up paper review section

### Phase 3: Visual Enhancement
1. Create custom CSS file for professional styling
2. Add professional headshot
3. Create project screenshots/demos
4. Design consistent visual theme
5. Implement responsive design

### Phase 4: Technical Features
1. Add PDF download functionality for CV
2. Implement project filtering/tags
3. Add publication citation export
4. Set up contact form
5. Add search functionality
6. Implement RSS feeds

### Phase 5: SEO & Professional Polish
1. Add meta descriptions
2. Implement structured data for publications
3. Create sitemap
4. Add analytics
5. Test all links and functionality
6. Performance optimization

## Website Structure Plan

```
/
├── index.html (Homepage)
├── about/
│   └── index.md (Extended bio and professional narrative)
├── cv/
│   ├── index.md (Web version)
│   └── cv.pdf (Downloadable version)
├── projects/
│   ├── _index.md (Projects overview)
│   ├── project-1/
│   ├── project-2/
│   └── project-3/
├── publications/
│   ├── _index.md (Publications list)
│   ├── papers/ (Academic papers)
│   └── reviews/ (Paper reviews and screenshots)
├── posts/ (Blog - long form)
│   ├── _index.md
│   └── [blog posts]
├── til/ (Today I Learned - short form)
│   ├── _index.md
│   └── [til entries]
└── contact/
    └── index.md
```

## Theme Customizations Needed

### 1. **Navigation Enhancement**
- Add top navigation bar for main sections
- Customize sidebar for better organization
- Add breadcrumb navigation

### 2. **Custom Layouts**
- Project showcase template
- Publication listing template
- CV/Resume template
- Homepage template

### 3. **Styling**
- Professional color scheme
- Typography improvements
- Better spacing and layout
- Mobile-responsive design

### 4. **New Shortcodes**
- Project card
- Publication citation
- Skill badge
- Timeline
- Paper screenshot gallery

## Content Best Practices

1. **Quality over Quantity**: Focus on 3-5 exceptional projects rather than many mediocre ones
2. **Clear Documentation**: Explain problems, solutions, and impact in accessible language
3. **Academic Integration**: Bridge technical and research work effectively
4. **Personal Branding**: Maintain consistent narrative across all sections
5. **Regular Updates**: Keep content fresh and relevant
6. **Accessibility**: Ensure all content is accessible and mobile-friendly

## Informational Interview Questions for About Page

### Professional Background:
1. What's your current role/position and field of study?
2. What are your main areas of expertise (e.g., machine learning, data science, specific research areas)?
3. What's your educational background (degrees, institutions, graduation years)?

### Technical Skills:
4. What programming languages are you proficient in?
5. What frameworks/tools do you use regularly?
6. What are your strongest technical accomplishments?

### Research & Academic Work:
7. What research topics are you most passionate about?
8. Do you have any published papers or ongoing research projects?
9. Have you presented at conferences or given talks?

### Career Goals:
10. What type of role are you targeting (industry research, academia, engineering)?
11. What makes you unique compared to other candidates?
12. What's your ideal work environment or company type?

### Personal Touch:
13. What got you interested in your field?
14. Any interesting side projects or hobbies related to your work?
15. How would you describe your approach to problem-solving?

## Technical Implementation Notes

### Hugo Configuration Updates Needed:
- Enable menu system for main navigation
- Configure taxonomies for tags and categories
- Set up output formats for RSS feeds
- Configure related content for blog posts

### Custom CSS Requirements:
- Professional typography system
- Color scheme for syntax highlighting
- Responsive grid system for projects
- Print styles for CV

### JavaScript Features:
- Search functionality
- Filter system for projects/publications
- Contact form validation
- Analytics integration

## Success Metrics

- Clean, professional appearance that loads quickly
- Easy navigation to key information
- Mobile-responsive design
- SEO-optimized for name searches
- Clear call-to-action for recruiters/contacts
- Demonstrates both technical depth and communication skills

## Next Steps

1. Answer the informational interview questions
2. Provide existing materials (CV, project descriptions, papers)
3. Confirm design preferences and priorities
4. Begin Phase 1 implementation with homepage and navigation structure