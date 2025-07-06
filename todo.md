# Personal Website Development Todo List

## Phase 0: Content Preparation (NEW - CURRENT PRIORITY)

### Complete Informational Interview
- [x] Professional background questions answered
- [x] Educational journey documented
- [x] Main areas of expertise identified
- [x] Create comprehensive interview-responses-detailed.md
- [ ] **IN PROGRESS: Technical skills section**
  - [ ] Development frameworks (Flask, FastAPI, testing frameworks)
  - [ ] DevOps/MLOps tools (Docker, CI/CD, code quality)
  - [ ] Research tools (Jupyter, cloud platforms)
- [ ] Strongest technical accomplishments (beyond MorphNet, tbp.floppy)
- [ ] Research topics and passion areas
- [ ] Career goals and target roles
- [ ] Personal touch questions (origin story, hobbies)
- [ ] Links and profiles (GitHub, LinkedIn, etc.)
- [ ] Teaching/mentoring experience
- [ ] Website tone preferences
- [ ] Key messages to convey

### Create Core Content Pages
- [ ] Write compelling About page using interview responses
- [ ] Create Research/Projects page featuring:
  - [ ] MorphNet project details
  - [ ] tbp.floppy package
  - [ ] Current work at Thousand Brains Project
- [ ] Draft initial blog posts:
  - [ ] "From Microfluidics to Machine Learning: My Journey"
  - [ ] "Understanding the Thousand Brains Theory"
  - [ ] Technical post about tbp.floppy or numpy internals
- [ ] Prepare professional headshot/avatar
- [ ] Write bio variations (short, medium, long)

## Phase 1: Research & Decision Making (AFTER CONTENT)

## Phase 1: Research & Decision Making

### Review Example Websites
- [ ] Visit and explore each Blowfish example site
  - [ ] nunocoracao.com - Note features you like/dislike
  - [ ] blowfish.page/users/ - Browse showcase gallery
  - [ ] Pay attention to: navigation, dark mode, animations, mobile experience
- [ ] Visit and explore each PaperMod example site
  - [ ] jessewei.dev - Understand why they migrated away
  - [ ] arkalim.github.io - Test search functionality
  - [ ] adityatelange.github.io/hugo-PaperMod/ - Explore all demo features
- [ ] Visit and explore Hugo Blox Academic examples
  - [ ] mickaellalande.github.io - Review academic features
  - [ ] matteocourthoud.github.io - Check research/blog balance
  - [ ] Only consider if you need heavy academic features

### Define Your Requirements
- [ ] List primary use cases for your site (blog, portfolio, about, etc.)
- [ ] Identify must-have features
  - [ ] Dark mode?
  - [ ] Search functionality?
  - [ ] Comments section?
  - [ ] Analytics?
  - [ ] Social media integration?
- [ ] Identify nice-to-have features
- [ ] Determine your technical comfort level
  - [ ] Comfortable with CSS customization?
  - [ ] Willing to learn Tailwind CSS (for Blowfish)?
  - [ ] Prefer minimal configuration?

### Make Theme Decision
- [ ] Based on research, choose between:
  - [ ] **Blowfish** - If you want modern design and extensive customization
  - [ ] **PaperMod** - If you want simplicity and proven reliability
  - [ ] **Hugo Book** - If you decide documentation structure fits your needs
  - [ ] **Other** - If you found something else appealing

## Phase 2: Preparation

### Backup Current Site
- [ ] Create a complete backup of current Hugo Book setup
  - [ ] `cp -r /Users/hlee/Desktop/hojaeklee /Users/hlee/Desktop/hojaeklee-backup-$(date +%Y%m%d)`
- [ ] Commit all current changes to git
  - [ ] `git add -A && git commit -m "Backup before theme migration"`
- [ ] Create a new branch for theme testing
  - [ ] `git checkout -b theme-migration`

### Content Audit
- [ ] List all current content files
- [ ] Identify any Hugo Book-specific shortcodes or features in use
- [ ] Note any custom CSS modifications in current theme
- [ ] Document current menu structure from hugo.toml

## Phase 3: Theme Installation (Choose One Path)

### Option A: If Choosing Blowfish
- [ ] Install Blowfish theme
  - [ ] Remove current theme: `git rm themes/hugo-book`
  - [ ] Add Blowfish: `git submodule add https://github.com/nunocoracao/blowfish themes/blowfish`
- [ ] Update hugo.toml
  - [ ] Change theme to "blowfish"
  - [ ] Review Blowfish configuration docs
- [ ] Copy example site configuration
  - [ ] `cp -r themes/blowfish/exampleSite/config/* ./config/`
- [ ] Install Blowfish CLI tool (optional but recommended)
  - [ ] `npm install -g @nunocoracao/blowfish-tools`

### Option B: If Choosing PaperMod
- [ ] Install PaperMod theme
  - [ ] Remove current theme: `git rm themes/hugo-book`
  - [ ] Add PaperMod: `git submodule add https://github.com/adityatelange/hugo-PaperMod themes/PaperMod`
- [ ] Update hugo.toml
  - [ ] Change theme to "PaperMod"
  - [ ] Add PaperMod-specific parameters
- [ ] Copy example configuration
  - [ ] Reference: themes/PaperMod/exampleSite/config.yml

### Option C: If Keeping Hugo Book
- [ ] Skip to Phase 5 for customization improvements

## Phase 4: Content Migration

### Basic Setup
- [ ] Test site builds: `hugo server -D`
- [ ] Fix any immediate build errors
- [ ] Verify home page displays

### Content Structure
- [ ] Migrate content from `/content/docs/` to appropriate new structure
  - [ ] Blowfish/PaperMod typically use `/content/posts/` for blog posts
  - [ ] May need `/content/about/` for about page
- [ ] Update front matter in content files
  - [ ] Remove Hugo Book-specific parameters
  - [ ] Add theme-specific parameters (tags, categories, etc.)

### Navigation & Menus
- [ ] Configure main menu in hugo.toml or config/_default/menus.toml
- [ ] Set up footer links
- [ ] Configure social media links

### Homepage Configuration
- [ ] For Blowfish: Choose between hero, profile, or custom layout
- [ ] For PaperMod: Choose between regular, profile, or home-info mode
- [ ] Configure homepage content/widgets

## Phase 5: Customization

### Visual Customization
- [ ] Set up color scheme/theme
- [ ] Configure dark/light mode preferences
- [ ] Add custom CSS if needed
  - [ ] Create `assets/css/custom.css`
  - [ ] Override theme variables

### Functionality
- [ ] Configure search (if supported)
- [ ] Set up comments system (if desired)
  - [ ] Disqus, Utterances, or Giscus
- [ ] Add analytics
  - [ ] Google Analytics or privacy-friendly alternatives
- [ ] Configure SEO settings

### Content Features
- [ ] Set up syntax highlighting preferences
- [ ] Configure table of contents behavior
- [ ] Set up social sharing buttons
- [ ] Configure RSS feeds

## Phase 6: Testing & Optimization

### Functionality Testing
- [ ] Test all internal links
- [ ] Verify search works (if implemented)
- [ ] Check responsive design on mobile devices
- [ ] Test dark/light mode switching
- [ ] Validate RSS feeds

### Performance
- [ ] Run `hugo --minify` for production build
- [ ] Check page load speeds
- [ ] Optimize images if needed
- [ ] Test with Google Lighthouse

### Cross-browser Testing
- [ ] Test in Chrome
- [ ] Test in Firefox
- [ ] Test in Safari
- [ ] Test in mobile browsers

## Phase 7: Deployment

### Final Preparations
- [ ] Update README.md with new theme information
- [ ] Document any custom modifications
- [ ] Clean up unused files from old theme

### Git Operations
- [ ] Commit all changes: `git add -A && git commit -m "Migrate to [theme name]"`
- [ ] Merge to main branch: `git checkout main && git merge theme-migration`
- [ ] Push to remote: `git push origin main`

### Deploy to GitHub Pages
- [ ] Verify GitHub Actions workflow works with new theme
- [ ] Check live site at https://hojaeklee.github.io/
- [ ] Monitor for any deployment issues

## Phase 8: Post-Migration

### Documentation
- [ ] Create a CHANGELOG.md noting the migration
- [ ] Document theme-specific customizations
- [ ] Note any features lost/gained in migration

### Future Enhancements
- [ ] List potential future customizations
- [ ] Research theme-specific plugins/extensions
- [ ] Plan content strategy for new theme capabilities

### Maintenance
- [ ] Set up process for theme updates
- [ ] Document how to update theme submodule
- [ ] Plan regular backups

---

## Notes

- Each phase should be completed before moving to the next
- Test frequently during migration - `hugo server -D`
- Keep the backup until you're completely satisfied
- Don't hesitate to ask for help in theme communities/forums
- Consider creating a test repository first if unsure

## Estimated Timeline

- Phase 1: 2-4 hours (research & decision)
- Phase 2: 1 hour (preparation)
- Phase 3: 1-2 hours (installation)
- Phase 4: 2-4 hours (content migration)
- Phase 5: 2-6 hours (customization - varies greatly)
- Phase 6: 1-2 hours (testing)
- Phase 7: 1 hour (deployment)
- Phase 8: Ongoing

**Total: 10-20 hours depending on customization level**