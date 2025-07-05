# 🌍 Interactive World Map - Travel Tracker

A beautiful, interactive web application to track countries you've visited and calculate your world coverage percentage.

![World Map Preview](https://img.shields.io/badge/Status-Ready%20to%20Deploy-brightgreen) ![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Compatible-blue) ![No Dependencies](https://img.shields.io/badge/Dependencies-None-orange)

## ✨ Features

- 🗺️ **Interactive World Map** - Real country boundaries using OpenStreetMap
- 🔍 **Smart Search** - Autocomplete with country flags and regions
- ⌨️ **Keyboard Navigation** - Full keyboard support (arrows, enter, escape)
- 📊 **Live Statistics** - Real-time world coverage percentage calculation
- 💾 **Export Options** - Download as SVG or high-resolution JPG
- 📱 **Mobile Friendly** - Responsive design for all devices
- ✨ **Beautiful UI** - Modern design with smooth animations

## 🚀 Quick Deploy to GitHub Pages

### Method 1: Upload Files (Easiest)

1. **Download this repository** as ZIP or clone it
2. **Create new GitHub repository**:
   - Go to [github.com](https://github.com) and click "New repository"
   - Name it something like `world-map-explorer` or `travel-tracker`
   - Make it **Public**
   - Check "Add a README file"
   - Click "Create repository"

3. **Upload files**:
   - Click "Add file" → "Upload files"
   - Drag and drop ALL files from this package
   - Commit with message: "Add Interactive World Map app"

4. **Enable GitHub Pages**:
   - Go to repository Settings → Pages (left sidebar)
   - Source: "Deploy from a branch"
   - Branch: "main" 
   - Folder: "/ (root)"
   - Click "Save"

5. **Access your live app**:
   - URL will be: `https://yourusername.github.io/repository-name`
   - Wait 2-5 minutes for deployment

### Method 2: Git Command Line

```bash
# Clone or download this repository
git clone https://github.com/yourusername/world-map-app.git
cd world-map-app

# Create your own repository on GitHub first, then:
git remote set-url origin https://github.com/yourusername/your-repo-name.git
git push -u origin main
```

Then follow step 4 above to enable GitHub Pages.

## 📁 Package Contents

```
world-map-app/
├── index.html          # Main application file
├── README.md          # This setup guide
├── CNAME              # Custom domain setup (optional)
└── .gitignore         # Git ignore file
```

## 🛠️ Customization

### Change Colors
Edit the CSS variables in `index.html`:
```css
/* Find these in the <style> section */
--primary-color: #667eea;
--secondary-color: #764ba2;
--accent-color: #48bb78;
```

### Add More Countries
Add entries to the `countryData` object in `index.html`:
```javascript
'Country Name': { 
    name: 'Display Name', 
    capital: 'Capital City', 
    area: 0.00, 
    region: 'Continent', 
    population: '000M', 
    iso: 'CC', 
    flag: '🏳️', 
    aliases: ['Alternative Names'] 
}
```

### Custom Domain (Optional)
1. Edit `CNAME` file with your domain: `worldmap.yourdomain.com`
2. Add CNAME record in your DNS: `yourusername.github.io`

## 🔧 Technical Details

- **No Build Process** - Works immediately after upload
- **No API Keys** - Uses free, public APIs only
- **Offline Ready** - Cached after first load
- **Cross-browser** - Works on all modern browsers
- **Lightweight** - Single HTML file under 100KB

### APIs Used (All Free)
- **OpenStreetMap** - Map tiles and country boundaries
- **Natural Earth** - Geographic data via GitHub CDN
- **Leaflet.js** - Interactive mapping library
- **HTML2Canvas** - Image export functionality

## 📱 Browser Support

- ✅ Chrome/Edge/Safari (latest)
- ✅ Firefox (latest)
- ✅ Mobile browsers (iOS/Android)
- ✅ Internet Explorer 11+

## 🐛 Troubleshooting

### Map not loading?
- Check internet connection
- Ensure GitHub Pages is enabled
- Wait 5 minutes after enabling Pages

### Countries not highlighting?
- Map data loads asynchronously
- Try refreshing the page
- Check browser console for errors

### Downloads not working?
- JPG downloads require modern browser
- SVG downloads work in all browsers
- Check popup blockers

## 📄 License

This project is open source and available under the MIT License. Feel free to use, modify, and distribute.

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes  
4. Push to the branch
5. Open a Pull Request

## 🎉 Credits

- **Map Data**: OpenStreetMap contributors
- **Country Boundaries**: Natural Earth
- **Icons**: Flag emojis from Unicode Consortium
- **Design**: Custom CSS with modern web standards

---

**Enjoy tracking your travels! 🗺️✈️**

For support or questions, please open an issue on GitHub.