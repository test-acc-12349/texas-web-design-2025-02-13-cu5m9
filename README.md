# Texas Web Design Landing Page - Maintenance Guide

This guide will help you maintain and customize the Texas Web Design landing page. Whether you're new to web development or need a quick reference, follow these instructions to make common updates safely and effectively.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Header Section
The header contains the company name and navigation menu. To update:

```html
<!-- Company Name -->
<a href="/" class="text-2xl font-bold bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
    Texas Web Design  <!-- Edit this text to change company name -->
</a>
```

#### Navigation Menu Items
To modify navigation links, locate this section:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Features</a>
    <!-- Add or modify menu items here -->
</div>
```

### Hero Section
Update the main headline and subheading:
```html
<h1 class="text-5xl md:text-6xl lg:text-7xl font-bold leading-tight mb-8 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
    Best Websites In Texas  <!-- Edit main headline here -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    Creating stunning, high-performance websites that drive results  <!-- Edit subheading here -->
</p>
```

### Understanding Tailwind Classes
Common classes used in this template:
- `text-{size}`: Controls text size (xl, 2xl, etc.)
- `font-{weight}`: Controls text weight (bold, semibold)
- `bg-{color}`: Sets background color
- `p-{size}`: Sets padding
- `m-{size}`: Sets margin
- `flex`: Creates flexible container
- `grid`: Creates grid layout

## Fixing Broken Links

### Current Link Inventory
1. Navigation Menu Links:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact</a>
```

2. Call-to-Action Links:
```html
<a href="https://twd.com" class="...">Get Started</a>
<!-- Update this URL to your actual domain -->
```

### Updating Links
To update any link:
1. Locate the `<a>` tag
2. Modify the `href` attribute
3. Test the link

Example:
```html
<!-- Before -->
<a href="https://twd.com">Get Started</a>

<!-- After -->
<a href="https://your-actual-domain.com">Get Started</a>
```

## Linking Privacy and Terms Pages

### Footer Links Section
Locate the Legal section in the footer:
```html
<div>
    <h4 class="text-lg font-semibold text-white mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Cookie Policy</a></li>
    </ul>
</div>
```

### Adding Policy Pages
1. Create your policy pages (privacy.html, terms.html)
2. Update the links in the footer:
```html
<!-- Update these href attributes -->
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Layout**
   - Check for missing closing tags
   - Verify Tailwind CSS classes are spelled correctly
   - Ensure the Tailwind CDN link is working

2. **Non-Working Links**
   - Verify file paths are correct
   - Check for typos in URLs
   - Ensure linked pages exist in the correct location

3. **Responsive Design Issues**
   - Check mobile-specific classes (md:, lg:, etc.)
   - Test on different screen sizes
   - Verify the viewport meta tag is present

### Need Help?
If you encounter issues:
1. Check the browser console for errors
2. Verify all files are in the correct directory
3. Ensure all required assets are properly linked
4. Test the page in multiple browsers

Remember to always backup your files before making changes, and test thoroughly after each modification.