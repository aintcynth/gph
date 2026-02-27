# Quick Start Guide

Get your portfolio site up and running in minutes!

## 🚀 Quick Setup

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/gph-main.git
cd gph-main
```

### 2. Open Locally
Simply open `index.html` in your browser:
```bash
# Windows
start index.html

# macOS
open index.html

# Linux
xdg-open index.html
```

### 3. Using a Local Server (Recommended)
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (with http-server)
npx http-server

# Then visit: http://localhost:8000
```

## ✏️ Customize Your Portfolio

### Update Personal Info
Edit these sections in `index.html`:

1. **Page Title**: Line 3
   ```html
   <title>Your Name - Portfolio</title>
   ```

2. **Hero Section**: Around line 50-55
   ```html
   <h1>I am <B class="name">YOUR NAME</B></h1>
   <h2>Your Title Here</h2>
   ```

3. **About Section**: Around line 65-75
   ```html
   <h4>Your Name, Age, Location</h4>
   <p>Your bio and background...</p>
   ```

4. **Contact Info**: Around line 245-250
   ```html
   <p><span class="glyphicon glyphicon-phone"></span> Your Phone</p>
   <p><span class="glyphicon glyphicon-envelope"></span> Your Email</p>
   ```

### Update Styles
Edit `style.css` to customize colors:

```css
/* Primary Color (currently teal green) */
--primary: #068747;

/* All sections with primary color:
   .logo-small
   .carousel-control
   .carousel-indicators
   .panel
   .navbar links
   And more...
*/
```

### Update Images
Replace these image files in the project:
- `logo.png` - Your logo for navbar
- `icon.png` - Favicon (website tab icon)
- `pp.jpg` - Profile picture
- `me1.png` - Hero background image
- `elem.jpg`, `hs.jpg`, `csu.jpg` - School photos

### Update Videos
Replace video file references in portfolio section:
- `myvid.MOV`
- `vlog.MOV`
- `dance.MOV`

## 📱 Test Responsive Design

### Browser DevTools
1. Open Developer Tools (F12 or Cmd+I)
2. Click Responsive Design Mode (Ctrl+Shift+M)
3. Test all breakpoints:
   - iPhone (375px)
   - iPad (768px)
   - Desktop (1200px+)

### Test Specific Devices
- [ ] iPhone SE (375px)
- [ ] iPhone 12 (390px)
- [ ] iPad (768px)
- [ ] Laptop (1366px)
- [ ] Desktop (1920px)

## 🌐 Deploy to GitHub Pages

### Step 1: Push to GitHub
```bash
git add .
git commit -m "Initial portfolio commit"
git push origin main
```

### Step 2: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings**
3. Scroll to **Pages** section
4. Select **Main** branch as source
5. Save

Your site will be live at: `https://yourusername.github.io/gph-main/`

## 🔗 Useful Links

- Update GitHub profile link: Find `https://www.facebook.com/...` in HTML and replace
- Update resume/CV links as needed
- Add social media links

## 📝 File Structure Reference

```
.
├── index.html          ← Main portfolio page
├── style.css           ← Custom styling
├── bootstrap.min.css   ← Bootstrap framework
├── README.md           ← Project documentation
├── LICENSE             ← License file
├── .gitignore          ← Git ignore rules
└── images/             ← All image assets
```

## 🎨 Color Scheme

- **Primary**: `#068747` (Teal Green)
- **Text**: `#818181` (Gray)
- **Headings**: `#303030` (Dark Gray)
- **Background**: `#f6f6f6` (Light Gray)

To change colors globally:
1. Find all instances of `#068747` in `style.css`
2. Replace with your preferred color

## ✅ Pre-Launch Checklist

- [ ] Updated all personal information
- [ ] Replaced all images with your own
- [ ] Updated contact details
- [ ] Tested on mobile (375px minimum)
- [ ] Tested on desktop (1200px+)
- [ ] Tested in Chrome, Firefox, Safari
- [ ] All links verified (internal & external)
- [ ] Forms tested for UX
- [ ] Images optimized for web
- [ ] No broken links in console
- [ ] Pushed to GitHub
- [ ] Enabled GitHub Pages

## 🚀 Going Live

### GitHub Pages (Free)
- Deployed automatically when you push to GitHub
- URL: `username.github.io/gph-main`

### Other Options
- **Netlify**: Drag & drop deployment
- **Vercel**: Git integration
- **Firebase Hosting**: Google's hosting
- **Heroku**: Full-stack deployment

## 🐛 Troubleshooting

### Website looks broken on mobile
- Clear browser cache
- Test in incognito/private window
- Check console for errors (F12)

### Images not showing
- Verify image file names match exactly
- Check file paths in HTML
- Ensure images are in the same folder

### Styles not applying
- Clear cache and reload (Ctrl+Shift+R)
- Check CSS file is linked in HTML
- Verify file path is correct

## 📚 Learn More

- [HTML Guide](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [CSS Guide](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [Bootstrap Docs](https://getbootstrap.com/)
- [Responsive Design](https://web.dev/responsive-web-design-basics/)

## 💡 Tips

1. **Backup First**: Before major changes, create a new branch
   ```bash
   git checkout -b updates
   ```

2. **Test Locally**: Always test before pushing to GitHub
   ```bash
   python -m http.server 8000
   ```

3. **Use Developer Tools**: Test responsive design with browser DevTools

4. **Keep it Updated**: Regularly update content and keep portfolio fresh

## 🤝 Need Help?

- Check [README.md](README.md) for full documentation
- Review [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines
- Open an issue on GitHub
- Check [CODE_STYLE.md](CODE_STYLE.md) for coding standards

---

**Happy coding! 🎉**

*Questions? Open an issue or reach out on GitHub*
