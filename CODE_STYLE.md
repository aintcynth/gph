# Code Style Guide

This document outlines the coding standards and best practices used in the Hiacynth Personal Portfolio project.

## HTML Standards

### Structure
- Use semantic HTML5 tags (`<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`, etc.)
- Proper nesting and indentation (2 spaces)
- Use lowercase for all HTML tags and attributes

### Best Practices
```html
<!-- Good -->
<img src="image.jpg" alt="Descriptive text" class="responsive-image">
<button type="submit" class="btn btn-primary">Send</button>

<!-- Avoid -->
<img src="image.jpg">
<input type="submit" value="Send">
```

### Accessibility
- Always include `alt` text for images
- Use proper heading hierarchy (h1-h6)
- Include `type` attribute on form inputs
- Use `<label>` with `for` attribute for form fields
- Ensure good color contrast

## CSS Standards

### Formatting
```css
/* Good */
.selector {
  property: value;
  property: value;
}

/* Avoid */
.selector{property:value;}
```

### Naming Conventions
- Use kebab-case for class names
- Use descriptive, semantic names
- Avoid single-letter names
- Group related styles together

```css
/* Good */
.button-primary { }
.form-group { }
.navbar-header { }

/* Avoid */
.bp { }
.fg { }
.btn1 { }
```

### Units
- Use `rem` for font sizes and spacing (based on 16px root)
- Use `%` for widths (responsive)
- Use `px` for borders
- Use `em` for relative sizing within components

```css
/* Good */
body {
  font-size: 1rem;
  margin-bottom: 2rem;
  border: 1px solid #ccc;
}

/* Avoid */
body {
  font-size: 16px;
  margin-bottom: 32px;
}
```

### Media Queries
- Follow mobile-first approach
- Use consistent breakpoints:
  - `max-width: 575px` - Extra small (phones)
  - `max-width: 767px` - Small (tablets)
  - `max-width: 991px` - Medium (small desktops)
  - `min-width: 1200px` - Large (large desktops)

```css
/* Mobile-first approach */
.element {
  width: 100%;  /* Default for mobile */
}

@media screen and (min-width: 768px) {
  .element {
    width: 50%;  /* For tablets and up */
  }
}
```

### Colors
- Use hex codes or rgb()
- Maintain consistent color palette
- Define colors in comments or variables

```css
/* Primary Color Theme */
--primary: #068747;
--secondary: #000000;
--text-dark: #303030;
--text-light: #818181;
--background-light: #f6f6f6;
```

### Performance
- Avoid `!important` unless absolutely necessary
- Use efficient selectors
- Group media queries
- Minimize specificity

## JavaScript Standards

### Style
```javascript
// Good
$(document).ready(function(){
  // Code here
});

// Variable naming
const navbarHeight = 60;
let isScrolled = false;

// Function naming
function handleScroll() { }
const scrollToSection = () => { };
```

### Comments
```javascript
// Use comments for complex logic
// Avoid obvious comments

// Good: Explains why, not what
// DelayScroll allows animations to complete before jumping
const delayScroll = 900;

// Avoid: States the obvious
// Set timeout to 900
const timeout = 900;
```

### jQuery Conventions
```javascript
// Cache jQuery objects
const $navbar = $('.navbar');
const $scrollElements = $('.slideanim');

// Use on() for event delegation
$(document).on('click', '.btn', function() {
  // Handle click
});
```

## File Organization

```
gph-main/
├── index.html          # Main HTML file
├── style.css           # All custom CSS
├── bootstrap.min.css   # Bootstrap framework
├── README.md           # Documentation
├── LICENSE             # License file
├── .gitignore          # Git ignore rules
├── CONTRIBUTING.md     # Contribution guidelines
├── CHANGELOG.md        # Version history
├── CODE_STYLE.md       # This file
└── [image assets]      # Media files
```

## Git Commit Messages

### Format
```
Type: Brief description (50 chars or less)

Longer explanation if needed (72 chars per line)
- Bullet points for multiple changes
- Keep it concise and clear

Fixes #123
```

### Types
- `feat:` New feature
- `fix:` Bug fix
- `refactor:` Code refactoring
- `style:` CSS/styling changes
- `docs:` Documentation
- `perf:` Performance improvement
- `chore:` Maintenance tasks

### Examples
```
feat: Add dark mode toggle

style: Improve button hover effects

fix: Correct navbar alignment on mobile devices

docs: Update installation instructions
```

## Testing Standards

### Before Committing
- [ ] Test on desktop browsers (Chrome, Firefox, Safari, Edge)
- [ ] Test on mobile browsers
- [ ] Test all responsive breakpoints
- [ ] Verify all links work
- [ ] Test form submission
- [ ] Check animations smooth
- [ ] Verify no console errors

### Responsive Testing
- Extra Large: 1400px+
- Large: 1000px - 1399px
- Medium: 768px - 999px
- Small: 576px - 767px
- Extra Small: < 576px

## Performance Guidelines

### Images
- Optimize before using
- Use appropriate formats (JPEG, PNG, WebP)
- Include responsive sizes

### CSS & JavaScript
- Minimize render-blocking resources
- Avoid unnecessary JavaScript
- Cache jQuery selectors

### Loading
- Use CDN for libraries
- Defer non-critical JavaScript
- Lazy load images if possible

## Accessibility Checklist

- [ ] All images have alt text
- [ ] Color contrast is sufficient (WCAG AA)
- [ ] Keyboard navigation works
- [ ] Form labels are associated
- [ ] Headings are in order
- [ ] Links have descriptive text
- [ ] Buttons have proper roles

## Documentation Standards

### README Requirements
- Clear project description
- Getting started section
- Technology stack
- Features list
- Deployment instructions
- Contact information

### Code Comments
```javascript
// ✓ Good: Comment why, not what
// Increase animation duration on mobile for better visibility
const mobileDuration = 1200;

// ✗ Bad: Obvious comments
// Set duration
const duration = 1000;
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Android)

## External Resources

- [MDN Web Docs](https://developer.mozilla.org/)
- [Bootstrap Documentation](https://getbootstrap.com/)
- [CSS Tips](https://css-tricks.com/)
- [Web Accessibility](https://www.w3.org/WAI/)

---

*Last Updated: 2026*

For questions or suggestions about these standards, please open an issue or contact the maintainers.
