
# 🎬 Praveen Singh - Video Editor Portfolio

A modern, responsive portfolio website showcasing professional video editing work and services.

[![Live Demo](https://img.shields.io/badge/Live-Demo-ff6b6b?style=for-the-badge)](https://praveensinghpro.github.io)
[![License](https://img.shields.io/badge/License-MIT-4ecdc4?style=for-the-badge)](LICENSE)

![Portfolio Preview](https://via.placeholder.com/1200x600/0a0a0a/ff6b6b?text=Portfolio+Preview)

---

## ✨ Features

- **Modern Design** - Clean, professional interface with premium typography
- **Fully Responsive** - Optimized for all devices (mobile, tablet, desktop)
- **Smooth Animations** - Engaging scroll animations and transitions
- **Portfolio Showcase** - Dynamic filterable project gallery
- **Contact Form** - Interactive form for client inquiries
- **Social Integration** - Direct links to all social platforms
- **SEO Optimized** - Meta tags and semantic HTML for better visibility
- **Fast Loading** - Optimized performance and minimal dependencies

---

## 🚀 Live Demo

Visit the live website: **[praveensingh.pro](https://praveensinghpro.github.io)**

---

## 🛠️ Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with CSS Grid & Flexbox
- **JavaScript (Vanilla)** - Interactive features and animations
- **Google Fonts** - Outfit & Space Grotesk typography
- **Font Awesome 6** - Icon library
- **GitHub Pages** - Hosting

---

## 📁 Project Structure

```
praveensinghpro.github.io/
├── index.html              # Main HTML file
├── css/
│   └── style.css          # Main stylesheet
├── js/
│   └── main.js            # JavaScript functionality
├── images/
│   ├── profile.jpg        # Profile picture
│   ├── project1.jpg       # Portfolio images
│   └── ...
├── videos/                # Video assets (optional)
├── README.md              # Project documentation
└── CNAME                  # Custom domain configuration
```

---

## 🎨 Color Palette

```css
Primary:    #ff6b6b  /* Coral Red */
Secondary:  #4ecdc4  /* Turquoise */
Dark BG:    #0a0a0a  /* Deep Black */
Light BG:   #1a1a1a  /* Dark Gray */
Text:       #ffffff  /* White */
Muted:      #b0b0b0  /* Light Gray */
```

---

## 📦 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/praveensinghpro/praveensinghpro.github.io.git
cd praveensinghpro.github.io
```

### 2. Customize Content

#### Update Personal Information

**index.html** - Update these sections:

```html
<!-- Social Links (Line ~48) -->
<a href="https://youtube.com/@yourhandle" target="_blank">

<!-- Contact Info (Line ~217) -->
<span>contact@praveensingh.pro</span>
<a href="tel:+919999999999">+91 99999 99999</a>
```

#### Add Your Images

```bash
# Add profile picture
images/profile.jpg

# Add portfolio project images
images/project1.jpg
images/project2.jpg
# etc...
```

#### Update Portfolio Projects

Replace the portfolio items in `index.html` with your actual projects:

```html
<div class="portfolio-item" data-category="youtube">
    <div class="portfolio-thumbnail">
        <img src="images/your-project.jpg" alt="Your Project">
        <div class="portfolio-overlay">
            <i class="fas fa-play"></i>
        </div>
    </div>
    <div class="portfolio-info">
        <h3>Your Project Title</h3>
        <p>Category • Details</p>
    </div>
</div>
```

### 3. Local Development

Simply open `index.html` in your browser:

```bash
# macOS
open index.html

# Linux
xdg-open index.html

# Windows
start index.html
```

Or use a local server:

```bash
# Python 3
python -m http.server 8000

# Node.js (with live-server)
npx live-server
```

Visit: `http://localhost:8000`

### 4. Deploy to GitHub Pages

```bash
# Add all changes
git add .

# Commit changes
git commit -m "Initial portfolio setup"

# Push to GitHub
git push origin main
```

**Enable GitHub Pages:**
1. Go to repository **Settings**
2. Navigate to **Pages**
3. Select **main** branch as source
4. Click **Save**

Your site will be live at: `https://praveensinghpro.github.io`

---

## 🌐 Custom Domain Setup

### Add Custom Domain (praveensingh.pro)

1. **Create CNAME file** in repository root:

```bash
echo "praveensingh.pro" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push
```

2. **Configure DNS Settings** with your domain provider:

**A Records** (Point to GitHub Pages):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**CNAME Record**:
```
www  →  praveensinghpro.github.io
```

3. **Enable HTTPS** in GitHub Pages settings (automatic after DNS propagation)

---

## ✏️ Customization Guide

### Change Colors

Edit `css/style.css`:

```css
:root {
    --primary-color: #your-color;
    --secondary-color: #your-color;
    --dark-bg: #your-color;
}
```

### Change Fonts

Replace Google Fonts in `index.html`:

```html
<link href="https://fonts.googleapis.com/css2?family=YourFont:wght@300;400;700&display=swap" rel="stylesheet">
```

Update in `css/style.css`:

```css
body {
    font-family: 'YourFont', sans-serif;
}
```

### Modify Animations

Adjust timing in `js/main.js`:

```javascript
// Change animation duration
el.style.transition = 'all 0.6s ease'; // Change to your preference
```

---

## 🎯 Portfolio Filtering

Projects are filtered by category using data attributes:

```html
data-category="youtube"
data-category="commercial"
data-category="short-form"
```

Add new categories in both HTML and JavaScript as needed.

---

## 📧 Contact Form Integration

The form currently shows an alert. To connect a backend:

### Option 1: Formspree (Recommended)

```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
    <input type="text" name="name" placeholder="Your Name" required>
    <input type="email" name="email" placeholder="Your Email" required>
    <textarea name="message" placeholder="Your Message" required></textarea>
    <button type="submit">Send Message</button>
</form>
```

### Option 2: Google Forms

1. Create a Google Form
2. Get the form action URL
3. Replace the form action in HTML

### Option 3: EmailJS

Add EmailJS library and configure in `js/main.js`

---

## 📱 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

---

## ⚡ Performance Optimization

- Optimized images (WebP format recommended)
- Lazy loading for images
- Minified CSS and JS (for production)
- CDN for external libraries
- Smooth scroll with CSS

### Recommended Image Sizes

```
Profile Picture:    500x500px
Portfolio Images:   1200x800px (16:10 ratio)
```

---

## 🔧 Troubleshooting

### Images Not Loading

```bash
# Check file paths
images/profile.jpg  # Correct
/images/profile.jpg # May cause issues on some servers
```

### Mobile Menu Not Working

Ensure JavaScript is loaded:

```html
<script src="js/main.js"></script> <!-- At bottom of body -->
```

### Animations Not Smooth

Enable hardware acceleration:

```css
.portfolio-item {
    transform: translateZ(0);
    will-change: transform;
}
```

---

## 📊 Analytics (Optional)

Add Google Analytics:

```html
<!-- Before </head> -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

---

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **Font Awesome** - Icon library
- **Google Fonts** - Typography
- **Unsplash** - Placeholder images
- **GitHub Pages** - Hosting

---

## 📞 Contact

**Praveen Singh**

- Website: [praveensingh.pro](https://praveensingh.pro)
- Email: contact@praveensingh.pro
- LinkedIn: [linkedin.com/in/praveensingh](https://linkedin.com/in/praveensingh)
- YouTube: [@praveensingh](https://youtube.com/@praveensingh)
- Instagram: [@praveensingh](https://instagram.com/praveensingh)

---

## 🔗 Related Projects

- [PixelTraivo](https://pixeltraivo.github.io) - YouTube Tools
- [CutVerge](https://cutverge.github.io) - Video Editing Resources

---

<div align="center">

**Made with ❤️ by Praveen Singh**

⭐ Star this repo if you found it helpful!

[Report Bug](https://github.com/praveensinghpro/praveensinghpro.github.io/issues) · [Request Feature](https://github.com/praveensinghpro/praveensinghpro.github.io/issues)

</div>
```

Now create it:

```bash
# Create README
cat > README.md << 'EOF'
[Paste the above content]
EOF

# Or create manually
touch README.md
# Then paste the content

# Commit
git add README.md
git commit -m "📝 Add comprehensive README documentation"
git push
```
