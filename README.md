# 💖 Will You Be My Valentine? 

An interactive, beautifully designed Valentine's Day web experience that tells a love story with stunning animations, memories, and an unforgettable moment.

**Live Demo:** https://valentine-eta-navy.vercel.app/

---

## ✨ Features

- 🎨 **Beautiful Gradient Design** - Smooth, romantic color transitions
- 🌙 **Dark/Light Theme Toggle** - Seamless theme switching
- ✨ **Animated Sparkle Cursor** - Interactive cursor effects
- 📸 **Memory Gallery** - Display your favorite photos and moments
- 🎬 **Video Background** - Smooth video integration with autoplay
- 💫 **Floating Hearts Animation** - Ambient romantic atmosphere
- 📱 **Fully Responsive** - Works perfectly on desktop, tablet, and mobile
- 🚀 **Performance Optimized** - Fast loading and smooth animations
- ♿ **Accessibility Focused** - Keyboard navigation and screen reader support
- 📊 **Scroll Progress Indicator** - Visual feedback as you explore

---

## 🚀 Getting Started

### Prerequisites
- A web browser (Chrome, Firefox, Safari, Edge)
- A text editor (VS Code, Sublime, Notepad++)
- Basic knowledge of HTML/CSS/JavaScript (optional)

### Installation & Setup

#### Option 1: Direct File Access
1. Clone or download this repository
   ```bash
   git clone https://github.com/iamgagantyagi/valentine.git
   cd valentine
   ```

2. Open `index.html` in your browser
   ```bash
   # On Windows (PowerShell)
   Start-Process index.html
   
   # On macOS
   open index.html
   
   # On Linux
   xdg-open index.html
   ```

#### Option 2: Using a Local Server (Recommended)

**Using Python 3:**
```bash
python -m http.server 8000
```
Then open: `http://localhost:8000`

**Using Node.js (Live Server):**
```bash
npm install -g live-server
live-server
```

**Using VS Code:**
1. Install "Live Server" extension
2. Right-click `index.html` → "Open with Live Server"

---

## 📝 Customization Guide

### Step 1: Replace Images
```bash
# Replace these files with your own photos:
- first_date.jpeg      # Your first date photo
- handshake_bond.jpeg  # A meaningful moment
- together_bond.jpeg   # A photo together
```

**Tips:**
- Keep images in portrait orientation for best results
- Use high-quality JPEGs (recommended size: 600x800px)
- Compress images to reduce load time
- Use tools like: TinyPNG, ImageOptim, or Squoosh

### Step 2: Replace the Video
```bash
# Replace this file with your own video:
- together_forever.mp4  # Your special video (20-60 seconds recommended)
```

**Video Guidelines:**
- Format: MP4 (H.264 codec)
- Resolution: 1920x1080 or higher
- Duration: 30-60 seconds ideal
- File size: Keep under 50MB for fast loading
- Use tools: FFmpeg, HandBrake, or DaVinci Resolve

### Step 3: Customize Text & Content

Open `index.html` in your text editor and find these sections:

#### Title & Heading
```html
<title>Will You Be My Valentine? 💖</title>
<!-- Change this to your custom title -->
```

#### Customize Messages
Search for text sections and modify:
- Main question/greeting
- Button text
- Celebration messages

#### Color Scheme
At the top of the CSS (lines 12-19), modify these variables:
```css
:root {
    --bg-gradient-start: #fce7f3;    /* Pink start */
    --bg-gradient-mid: #f3e8ff;      /* Purple middle */
    --bg-gradient-end: #ffe4e6;      /* Rose end */
    --primary-pink: #ec4899;         /* Accent pink */
    --primary-purple: #a855f7;       /* Accent purple */
}
```

**Color Palette Suggestions:**
- Red Theme: `#dc2626`, `#991b1b`
- Blue Theme: `#3b82f6`, `#1e3a8a`
- Green Theme: `#10b981`, `#065f46`
- Gold Theme: `#f59e0b`, `#92400e`

### Step 4: Deploy Online

#### Deploy to Vercel (Recommended - Free)
1. Push code to GitHub
2. Visit [vercel.com](https://vercel.com)
3. Click "New Project"
4. Select your GitHub repository
5. Click "Deploy"

**That's it!** Your site goes live instantly.

#### Deploy to Netlify (Free Alternative)
1. Push code to GitHub
2. Visit [netlify.com](https://netlify.com)
3. Click "New site from Git"
4. Select repository and deploy

#### Deploy to GitHub Pages
1. In your repository settings → Pages
2. Select main branch as source
3. Your site will be live at: `username.github.io/valentine`

---

## 📱 Mobile Optimization

This site is fully responsive! Here's what's optimized:

- ✅ Touch-friendly buttons and interactions
- ✅ Optimized text sizes for readability
- ✅ Fast load times on 4G networks
- ✅ Smooth animations on mobile
- ✅ Proper viewport settings

**Testing on Mobile:**
1. Open on your phone/tablet browser
2. Test all buttons and interactions
3. Check video playback
4. Verify images load correctly

---

## 🎨 Advanced Customization

### Add Music/Audio
Add this inside the `<body>` tag:
```html
<audio id="bgMusic" autoplay loop volume="0.3">
    <source src="your-song.mp3" type="audio/mpeg">
</audio>
```

### Add More Photos
Find the gallery section and add:
```html
<div class="memory-card">
    <img src="your-photo.jpeg" alt="description">
    <h3>Special Moment</h3>
</div>
```

### Change Animation Speed
In CSS, find `@keyframes` sections and modify `duration`:
```css
animation: float 15s infinite ease-in-out;
/* Change 15s to your preferred duration */
```

### Customize Font
Replace the Google Font link in `<head>`:
```html
<link href="https://fonts.googleapis.com/css2?family=YOUR+FONT:wght@400;600;700&display=swap" rel="stylesheet">
```

---

## 🔒 Privacy & Security

- ✅ No user data is collected
- ✅ No cookies or tracking
- ✅ All files are static HTML/CSS/JS
- ✅ Safe to share publicly
- ✅ Works offline (once loaded)

---

## 🐛 Troubleshooting

### Video Not Playing
- ✅ Check file format (must be MP4)
- ✅ Verify file path is correct
- ✅ Try reloading the page
- ✅ Check browser supports HTML5 video
- ✅ Reduce video file size

### Images Not Loading
- ✅ Check image file names match exactly (case-sensitive)
- ✅ Verify file paths are correct
- ✅ Use forward slashes `/` not backslashes
- ✅ Check image format (JPEG/PNG supported)

### Animations Not Smooth
- ✅ Close other browser tabs
- ✅ Update your browser
- ✅ Check GPU acceleration is enabled
- ✅ Reduce number of floating hearts

### Page Loads Slowly
- ✅ Optimize image file sizes
- ✅ Compress video file
- ✅ Use a Content Delivery Network (CDN)
- ✅ Enable browser caching

---

## 📊 File Structure

```
valentine/
├── index.html              # Main HTML file
├── first_date.jpeg         # Photo 1
├── handshake_bond.jpeg     # Photo 2
├── together_bond.jpeg      # Photo 3
├── together_forever.mp4    # Video (hidden from public view)
├── README.md               # This file
└── .gitignore             # Hides sensitive files from git
```

---

## 🎯 Share Your Creation

### Instagram
```
Check out this Valentine's experience! 💖
Perfect for sharing your love story 💕
✨ Interactive & Beautiful ✨
```

### Twitter/X
```
Just created an interactive Valentine experience! 💖
Share your love story in style ✨
https://valentine-eta-navy.vercel.app
```

### WhatsApp/Messenger
```
🎬✨ Check out this special Valentine experience I created! 💖
https://valentine-eta-navy.vercel.app
```

---

## 💡 Ideas for Use

- 💍 **Proposal** - Create a proposal moment
- 👰 **Wedding** - Celebrate your wedding day
- 💑 **Anniversary** - Celebrate your love
- 🎂 **Birthday** - Make someone's day special
- 🎓 **Graduation** - Celebrate achievements
- 👨‍👩‍👧 **Family** - Share family memories
- 💌 **Confession** - Share your feelings

---

## 🤝 Contributing

Want to improve this project? Feel free to:
- Report bugs
- Suggest features
- Create pull requests
- Share your customizations

---

## 📄 License

This project is open source and available under the MIT License.

---

## 🎓 Learning Resources

Improve your web development skills:
- [MDN Web Docs](https://developer.mozilla.org/)
- [CSS Tricks](https://css-tricks.com/)
- [JavaScript.info](https://javascript.info/)
- [Codecademy](https://codecademy.com/)

---

## 📞 Support

Having issues? 
- Check the Troubleshooting section above
- Review the code comments in `index.html`
- Visit [MDN Documentation](https://developer.mozilla.org/)

---

## 🙏 Credits

Created with ❤️ for love and special moments.

---

## 🔄 Updates & Versions

**v1.0** - Initial release with core features
- Interactive design
- Dark/Light theme
- Smooth animations
- Mobile responsive

**Coming Soon:**
- Multiple language support
- Custom music integration
- Social media sharing buttons
- Gallery animations

---

**Made with 💖 and code | Last Updated: February 2026**

For more projects and creations, visit: https://github.com/iamgagantyagi
