# Delightful Bean Landing Page - Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the Delightful Bean coffee cart landing page. Written for beginners, it covers essential updates and modifications you'll need to make.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Hero Section
The main headline and subtitle are located in the first `section` tag after `<main>`:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold tracking-tight leading-tight mb-6">
    St. Petersburg Wedding Coffee Cart
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    Making your St. Pete wedding day even more memorable
</p>
```

To modify:
1. Replace the text between the `<h1>` tags for the main headline
2. Update the text between the `<p>` tags for the subtitle
3. The classes like `text-4xl` control text size - larger numbers mean bigger text

### Feature Cards
Located in the "Premium Coffee Experience" section, each feature card follows this structure:

```html
<div class="bg-gray-50 rounded-2xl p-8 hover:shadow-lg transition-shadow duration-300">
    <h3 class="text-xl font-semibold mb-4">Craft Drinks</h3>
    <p class="text-gray-600">Expertly crafted coffee beverages...</p>
</div>
```

To modify:
1. Find the feature cards in the `#features` section
2. Update the `<h3>` text for the feature title
3. Modify the `<p>` text for the feature description
4. Keep the existing classes to maintain styling

### Understanding Tailwind Classes
Common classes used throughout:
- `text-gray-600`: Sets text color to gray
- `mb-4`: Adds margin bottom (spacing)
- `px-6`: Adds horizontal padding
- `py-4`: Adds vertical padding
- `rounded-lg`: Rounds corners
- `hover:`: Prefix for hover effects

## Managing Links

### Navigation Menu Links
Located in the header section:

```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Services</a>
    <a href="#benefits" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Benefits</a>
    <!-- More links -->
</div>
```

To update:
1. Locate the `<a>` tags within the navigation
2. Change the `href` attribute to point to your new destination
3. Update the link text between the `<a>` tags
4. Keep the existing classes for consistent styling

### External Links
The main call-to-action button links:

```html
<a href="https://www.delightfulbean.com/" class="inline-block bg-gray-900 text-white px-8 py-4 rounded-lg">
    Book Your Date
</a>
```

To modify:
1. Update the `href` attribute with your booking URL
2. Ensure the URL includes `https://` or `http://`
3. Test the link after updating

### Social Media Links
Located in the footer:

```html
<div class="flex space-x-4">
    <a href="#" class="text-gray-600 hover:text-gray-900">Instagram</a>
    <a href="#" class="text-gray-600 hover:text-gray-900">Facebook</a>
</div>
```

Replace the `#` with your actual social media URLs.

## Adding Privacy and Terms Pages

### Footer Legal Links
Located at the bottom of the page:

```html
<div>
    <h3 class="text-lg font-semibold mb-4">Legal</h3>
    <div class="space-y-2">
        <a href="#" class="block text-gray-600 hover:text-gray-900">Privacy Policy</a>
        <a href="#" class="block text-gray-600 hover:text-gray-900">Terms of Service</a>
    </div>
</div>
```

To link privacy and terms pages:
1. Create `privacy.html` and `terms.html` in your root directory
2. Update the href attributes:
```html
<a href="privacy.html" class="block text-gray-600 hover:text-gray-900">Privacy Policy</a>
<a href="terms.html" class="block text-gray-600 hover:text-gray-900">Terms of Service</a>
```

## Troubleshooting

Common issues and solutions:

### Broken Links
- Ensure all URLs start with `http://`, `https://`, or `/`
- For internal links (same website), use relative paths (`./privacy.html`)
- Test all links after updating

### Styling Issues
- Don't remove Tailwind classes unless you're sure about the impact
- Keep responsive classes (starting with `md:` or `lg:`)
- If text looks wrong, check for missing closing tags

### Text Updates
- Always maintain the HTML structure when updating text
- Keep existing classes when replacing content
- Test responsiveness after major text changes

Need more help? Contact your web developer or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).