# Mustang Workshop Manuals Landing Page - Maintenance Guide

This guide will help you maintain and customize the Mustang Workshop Manuals landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common maintenance tasks.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the main navigation and logo. To update:

1. **Logo Text:**
```html
<!-- Find this section in the header -->
<a href="#" class="text-2xl font-bold bg-gradient-to-r from-blue-500 to-purple-600 bg-clip-text text-transparent">
    Mustang Manuals  <!-- Change this text -->
</a>
```

2. **Navigation Links:**
```html
<div class="hidden md:flex space-x-8">
    <!-- Update these link texts as needed -->
    <a href="#features" class="text-gray-300 hover:text-white transition-colors duration-300">Features</a>
    <a href="#benefits" class="text-gray-300 hover:text-white transition-colors duration-300">Benefits</a>
</div>
```

### Hero Section
Located at the top of the page:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-6 bg-gradient-to-r from-blue-500 to-purple-500 bg-clip-text text-transparent">
    Ford Mustang Workshop Manuals  <!-- Main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-300 mb-8">
    Mustang PDF Manuals for Auto Repair & Maintenance  <!-- Subheadline -->
</p>
```

### Tailwind CSS Tips
- `text-{size}`: Controls font size (e.g., `text-xl`, `text-2xl`)
- `md:text-{size}`: Applies styles at medium screen sizes
- `mb-{number}`: Sets margin bottom (e.g., `mb-8` = 2rem)
- `bg-gray-900`: Sets background color
- `hover:scale-105`: Enlarges element on hover

## Managing Links

### Navigation Menu Links
Current internal links that need checking:

```html
<!-- In the navigation menu -->
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

To update links:
1. For internal sections, use `#section-id`
2. For external pages, use full URL:
```html
<a href="https://your-domain.com/page">Link Text</a>
```

### Call-to-Action Buttons
Update the main CTA links:

```html
<!-- Find this button in the hero section -->
<a href="https://carmanuals.org/shop/?make=Ford&model=Mustang" class="inline-flex items-center justify-center px-8 py-4 bg-gradient-to-r from-blue-600 to-purple-600 rounded-full">
    Download Manual
</a>
```

## Adding Privacy and Terms Pages

### 1. Create New Pages
Create two new files in your root directory:
- `privacy.html`
- `terms.html`

### 2. Update Footer Links
Replace the placeholder links in the footer:

```html
<!-- Find this section in the footer -->
<div>
    <h3 class="text-xl font-bold mb-4">Legal</h3>
    <ul class="space-y-2">
        <!-- Update these href attributes -->
        <li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors">Privacy Policy</a></li>
        <li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors">Terms of Service</a></li>
    </ul>
</div>
```

### 3. Maintain Consistent Styling
Copy these classes for new links to maintain consistency:
```html
class="text-gray-400 hover:text-white transition-colors"
```

## Troubleshooting

Common issues and solutions:

### Broken Links
- Check for typos in `href` attributes
- Ensure file names match exactly (case-sensitive)
- Verify file locations relative to index.html

### Styling Issues
- Check for missing Tailwind classes
- Verify class names are spelled correctly
- Ensure responsive classes (md:, lg:) are in correct order

### Layout Problems
- Check container classes: `container mx-auto px-4`
- Verify padding classes: `py-24 px-4`
- Check responsive classes for different screen sizes

Need additional help? Contact technical support or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).