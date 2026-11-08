# School Project Website

A multi-page educational website built with HTML5, CSS3, and vanilla JavaScript. The layout mimics a digital textbook manual with a fixed sidebar navigation and dynamic content area.

## Project Structure

```
HTML School/
├── index.html              # Homepage
├── css/
│   └── styles.css          # Main stylesheet
├── js/
│   └── main.js             # JavaScript functionality
├── pages/
│   ├── about.html          # About Us page
│   ├── purpose.html        # Purpose page
│   ├── special-thanks.html # Special Thanks page
│   ├── references.html     # References page
│   └── lessons.html        # Lessons page
├── assets/
│   └── images/
│       └── placeholder-logo.svg  # Placeholder logo
└── README.md               # This file
```

## Features

- **Fixed Sidebar Navigation**: Easy access to all pages from any section
- **Responsive Design**: Mobile-friendly with hamburger menu toggle
- **Warm Color Scheme**: Light orange/cream headers with white cards
- **Clean Typography**: Modern, readable fonts
- **Organized Structure**: Easy to customize and expand
- **Top Logos Section**: 3 logos displayed at the top of each page
- **Footer Logo**: Logo displayed on the left side of the footer

## How to Use

1. **Open the Website**: Simply open `index.html` in a web browser (Chrome, Firefox, Edge, etc.)

2. **Navigate**: Click on any link in the sidebar to move between pages

3. **Mobile View**: On smaller screens, click the hamburger menu (☰) to toggle the navigation

## Customization Guide

### Changing the Logo

Replace `assets/images/placeholder-logo.svg` with your own school logo. The logo should be:
- Recommended size: 80x80 pixels (or similar square aspect ratio)
- Format: SVG, PNG, or JPG
- Name your file: `logo.svg` (or update the path in all HTML files)

### Customizing the Top Logos Section

Each page has 3 logos at the top. To customize them:

1. **Replace the logos**: Update the image sources in the top-logos section of each HTML file
2. **Change the labels**: Modify the `<span>` text below each logo (e.g., "School", "Education", "Learning")
3. **Add different logos**: You can use different logo images for each of the 3 positions

Example from index.html:
```html
<div class="top-logos">
    <div class="top-logo-item">
        <img src="assets/images/placeholder-logo.svg" alt="Logo 1">
        <span>School</span>
    </div>
    <div class="top-logo-item">
        <img src="assets/images/placeholder-logo.svg" alt="Logo 2">
        <span>Education</span>
    </div>
    <div class="top-logo-item">
        <img src="assets/images/placeholder-logo.svg" alt="Logo 3">
        <span>Learning</span>
    </div>
</div>
```

### Customizing the Footer Logo

The footer has a logo on the left side. To customize:
- Update the image source in the footer section of each HTML file
- Change the text next to the logo by modifying the `<span>` content

Example:
```html
<div class="footer-logo">
    <img src="assets/images/placeholder-logo.svg" alt="School Logo">
    <span>School Project</span>
</div>
```

### Modifying Colors

Edit the CSS variables in `css/styles.css` (lines 8-14):

```css
:root {
    --primary-orange: #FF9800;      /* Main accent color */
    --secondary-orange: #FFB74D;    /* Lighter accent */
    --cream-bg: #FFF3E0;            /* Background color */
    --light-cream: #FFE0B2;         /* Header background */
    --white: #FFFFFF;               /* Card background */
    --text-dark: #333333;           /* Main text color */
    --text-light: #666666;          /* Secondary text color */
    --shadow: rgba(0, 0, 0, 0.1);   /* Shadow color */
    --sidebar-width: 250px;         /* Sidebar width */
}
```

### Adding Content

Each page has a content card section where you can add your own text, images, and other content:

```html
<div class="content-card">
    <div class="content-body">
        <h2>Your Heading</h2>
        <p>Your content goes here...</p>
    </div>
</div>
```

### Adding New Pages

1. Create a new HTML file in the `pages/` folder
2. Copy the structure from an existing page (e.g., `about.html`)
3. Update the page title and content
4. Add a link to the new page in the sidebar navigation in all HTML files
5. Update the JavaScript to handle the new page's active state

### Changing Navigation Links

To add, remove, or rename navigation links, update the sidebar in every HTML file:

```html
<nav class="sidebar-nav">
    <ul>
        <li><a href="../index.html">Home Page</a></li>
        <li><a href="about.html">About Us</a></li>
        <!-- Add or remove links here -->
    </ul>
</nav>
```

## Technologies Used

- **HTML5**: Semantic markup and structure
- **CSS3**: Styling, responsive design, and animations
- **Vanilla JavaScript**: Mobile menu toggle and active state management
- **SVG**: Scalable graphics for the logo

## Browser Compatibility

Works on all modern browsers:
- Chrome (recommended)
- Firefox
- Edge
- Safari

## Responsive Breakpoints

- **Desktop**: > 768px (fixed sidebar)
- **Mobile/Tablet**: ≤ 768px (hamburger menu)

## Tips for Students

1. **Save Your Work**: Always save files before testing in the browser
2. **Test Regularly**: Open your HTML files in a browser after making changes
3. **Use Browser Tools**: Press F12 to open developer tools for debugging
4. **Keep Backups**: Copy your work before making major changes
5. **Organize Your Content**: Use clear headings and structure in your content
6. **Check Links**: Ensure all navigation links work correctly
7. **Test on Mobile**: Resize your browser to test the mobile view

## File Path Notes

- Files in the `pages/` folder use `../` to reference the parent directory
- Example: `../css/styles.css` (from pages folder)
- Example: `css/styles.css` (from root directory)

## Need Help?

If you encounter issues:
1. Check that all file paths are correct
2. Ensure the CSS and JS files are linked properly
3. Verify that the folder structure matches the setup
4. Test in a different browser if something doesn't display correctly

## License

This project is created for educational purposes. Feel free to modify and use it for your school projects.
