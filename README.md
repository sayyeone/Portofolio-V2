# Portfolio-V2

A modern, elegant personal portfolio website showcasing web development projects. Clean design with gradient effects, smooth animations, and fully responsive layout.

**Live Demo:** [Portfolio-V2.github.io](https://sayyeone.github.io/Portfolio-V2)

## What's This?

This is a complete personal portfolio website featuring a beautiful gradient design with blurred blob backgrounds, interactive project cards with modal popups, and smooth scrolling navigation. Perfect for showcasing your skills, projects, and professional information to potential employers or clients.

## Tech Stack

Keep it simple:
* HTML5 & CSS3
* Tailwind CSS (via CDN)
* Vanilla JavaScript
* Google Fonts (Inter)
* Custom gradient effects
* Modal popups

No build tools or complex setup required. Just download and go.

## Getting Started

**Option 1: Just open it**

Clone the repo and double-click `index.html`. Done.

```bash
git clone https://github.com/sayyeone/portfolio.git
cd portfolio
# Double click index.html
```

**Option 2: Use Live Server (recommended)**

If you're using VS Code:
1. Install the Live Server extension
2. Right click `index.html` → Open with Live Server
3. Browser opens automatically at `localhost:5500`

**Option 3: Python server**

```bash
python -m http.server 8000
# Open http://localhost:8000 in your browser
```

## Deploying to GitHub Pages

Want to put this online? Super easy.

1. Push your code to GitHub:
```bash
git add .
git commit -m "initial commit"
git push origin main
```

2. Go to your repo → Settings → Pages
3. Under "Source", select `main` branch and `/ (root)` folder
4. Hit Save and wait a minute

Your site will be live at `https://yourusername.github.io/portfolio`

**Custom Domain**

Got your own domain? Create a `CNAME` file with your domain:
```
yourdomain.com
```

Then configure DNS with your domain provider. Wait 24 hours for propagation.

## Customizing

Everything's straightforward to customize.

**Change colors:** Edit the gradient colors in `style.css`:

```css
/* Main gradient: pink to orange */
.gradient-text {
    background: linear-gradient(135deg, #ec4899 0%, #f97316 100%);
}

/* Update gradient blobs */
.blob-1 {
    background: linear-gradient(135deg, #fce7f3 0%, #fbcfe8 100%);
}
```

**Update profile images:** Replace these files in your project:
```
img/profile-img.jpg      # Hero section profile
img/profile-about.jpg    # About section image
```

**Add your projects:** Edit the project cards in `index.html`:

```html
<div class="project-card" onclick="openModal('modal1')">
    <img src="img/your-project.png" alt="Your Project">
    <h3>Your Project Name</h3>
    <p>Your project description</p>
</div>
```

**Update modal content:** Modify the modal sections for each project:

```html
<div id="modal1" class="modal">
    <div class="modal-content">
        <img src="img/your-project.png" alt="Your Project">
        <h2>Your Project Name</h2>
        <p>Detailed description...</p>
        <a href="https://github.com/yourusername/project">View on GitHub</a>
    </div>
</div>
```

**Modify your information:** Update text in `index.html`:
- Name and title in hero section
- About me description
- Skills tags
- Education details
- Contact information
- Social media links

## Project Structure

```
portfolio/
├── index.html          # Main portfolio page
├── style.css           # Custom styles & animations
├── script.js           # JavaScript functionality
├── img/                # Image assets
│   ├── profile-img.jpg
│   ├── profile-about.jpg
│   ├── distreaming.png
│   ├── dinetfliks.png
│   └── bright.png
└── README.md           # You're reading it
```

Clean structure - easy to understand and modify.

## Features

* **Hero Section** - Eye-catching introduction with profile photo and gradient text
* **Blurred Gradient Background** - Beautiful animated blob effects
* **About Section** - Professional introduction with skills showcase
* **Interactive Project Cards** - Hover effects with smooth transitions
* **Modal Popups** - Netflix-style project details on click
* **Education Timeline** - Clean display of educational background
* **Contact Form** - Built-in contact form with styled inputs
* **Social Links** - Quick access to GitHub, LinkedIn, and email
* **Smooth Scrolling** - Seamless navigation between sections
* **Fully Responsive** - Perfect on desktop, tablet, and mobile
* **Keyboard Navigation** - Close modals with Escape key

## Modal Features

The project cards feature interactive modals that:
- Open with smooth fade-in and scale animation
- Display full project image
- Show detailed description
- Include technology tags
- Provide direct GitHub link
- Close via button, backdrop click, or Escape key
- Prevent body scroll when open

## Customization Tips

**Adding more projects:**

1. Add a new project card in the grid
2. Create a corresponding modal with unique ID
3. Update the `onclick` attribute to match modal ID
4. Add project image to `img/` folder

**Changing font:**

Replace the Google Fonts import in `index.html`:
```html
<link href="https://fonts.googleapis.com/css2?family=YourFont:wght@300;400;700&display=swap">
```

Update CSS:
```css
* {
    font-family: 'YourFont', sans-serif;
}
```

**Adjusting gradient blobs:**

Modify blob positions and colors in `style.css`:
```css
.blob-1 {
    width: 600px;
    height: 600px;
    top: -200px;
    left: -200px;
    background: linear-gradient(135deg, #yourcolor1, #yourcolor2);
}
```

## Browser Support

Works flawlessly on all modern browsers:
* Chrome (latest)
* Firefox (latest)
* Safari (latest)
* Edge (latest)
* Mobile browsers

## Performance

- Lightweight and fast loading
- Minimal external dependencies
- Optimized images recommended (compress before upload)
- Smooth 60fps animations
- No JavaScript frameworks needed

## Tips for Best Results

1. **Optimize images** - Use tools like TinyPNG to compress images
2. **Use high-quality project screenshots** - Recommended size: 769x414px
3. **Keep descriptions concise** - Short, impactful text works best
4. **Update regularly** - Add new projects as you create them
5. **Test on mobile** - Ensure everything looks great on small screens
6. **Personalize colors** - Make it match your personal brand

## SEO Tips

Add these to your `index.html` for better SEO:

```html
<meta name="description" content="Adisty Fatika Ardani - Computer Science Student & Web Developer Portfolio">
<meta name="keywords" content="web developer, portfolio, computer science, HTML, CSS, JavaScript">
<meta name="author" content="Adisty Fatika Ardani">
```

## Credits

* Design by Adisty Fatika Ardani
* Tailwind CSS for utility classes
* Inter font by Google Fonts
* Icons from Heroicons (via SVG)

## License

Feel free to use this template for your own portfolio. Attribution appreciated but not required.

---

Made with ❤️ by [Adisty Fatika Ardani](https://github.com/sayyeone)

Questions? Open an issue or reach out directly!
