# 🔥 Lava Background Embed Generator

A Windows XP-themed embed generator that creates stunning fullscreen lava backgrounds for CRM systems and web applications. Features an authentic retro interface with modern functionality.

## ✨ Features

### 🎨 **Background Presets**
- **Ticket Hub** - Orange/green lava animation
- **Dashboard** - Blue lava animation  
- **Coming Soon** - Additional presets in development

### 🖥️ **Windows XP Interface**
- Authentic Windows XP styling with Tahoma fonts
- Classic title bar with gradient effects
- Functional window controls (close button)
- Fully draggable window interface

### 📱 **Mobile Responsive**
- Touch-friendly interactions
- Adaptive layout for all screen sizes
- Optimized touch targets (44px minimum)
- Unified mouse and touch event handling

### 🚀 **Easy Integration**
- One-click embed code generation
- Dynamic URL detection
- Copy-to-clipboard functionality
- Fullscreen iframe implementation

## 🛠️ Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Poupun/LavaBackground-Generator.git
   cd LavaBackground-Generator
   ```

2. **Open in your web server:**
   - For local development: Open `index.html` in your browser
   - For production: Deploy to your web server

3. **Required files:**
   ```
   index.html          # Main application
   styles.css          # Windows XP theme styling
   lavaembed.html      # Orange lava animation
   embedlava-blue.html # Blue lava animation
   ```

## 🎯 Usage

### **Generating Embed Codes**

1. **Select a Preset:**
   - Choose from available background animations
   - Preview appears in the preset grid

2. **Generate Code:**
   - Click "Generate Embed Code"
   - Copy the generated iframe code

3. **Integrate:**
   ```html
   <!-- Example generated code -->
   <iframe src="https://yoursite.com/lavaembed.html" 
           width="100%" 
           height="100%" 
           frameborder="0" 
           style="position: fixed; top: 0; left: 0; width: 100vw; height: 100vh; z-index: -1; pointer-events: none;">
   </iframe>
   ```

### **Window Controls**

- **🖱️ Dragging:** Click and drag the title bar to move the window
- **📱 Touch:** Touch and drag on mobile devices
- **❌ Close:** Click the X button to close (with confirmation)
- **📍 Position:** Starts in top-right corner on desktop, full-width on mobile

## 🎨 Customization

### **Adding New Presets**

1. **Create animation file** (e.g., `my-animation.html`)

2. **Update preset configuration:**
   ```javascript
   const presets = {
       'my-preset': {
           name: 'My Preset',
           file: 'my-animation.html'
       }
   };
   ```

3. **Add preset item to HTML:**
   ```html
   <div class="xp-preset-item" data-preset="my-preset">
       <div class="xp-preset-preview">
           <div class="preset-my-animation"></div>
       </div>
       <div class="xp-preset-label">My Preset</div>
   </div>
   ```

### **Styling Modifications**

The Windows XP theme can be customized in `styles.css`:

- **Window colors:** Modify `.xp-window` background
- **Title bar:** Update `.xp-titlebar` gradient
- **Preset previews:** Customize `.preset-*` classes
- **Mobile responsiveness:** Adjust `@media` queries

## 📂 File Structure

```
LavaBackground-Generator/
├── index.html              # Main application interface
├── styles.css              # Windows XP theme & responsive styles
├── lavaembed.html          # Orange lava background animation
├── embedlava-blue.html     # Blue lava background animation
└── README.md               # This documentation
```

## 🔧 Technical Details

### **Dependencies**
- Font Awesome 6.4.0 (CDN)
- No JavaScript frameworks required
- Pure HTML/CSS/JavaScript implementation

### **Browser Support**
- ✅ Chrome 80+
- ✅ Firefox 75+
- ✅ Safari 13+
- ✅ Edge 80+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

### **Features Implementation**
- **Dragging:** Native DOM manipulation with transform positioning
- **Touch Support:** Unified mouse/touch event handling
- **Responsive:** CSS Grid and Flexbox with mobile-first approach
- **Clipboard:** Modern Clipboard API with fallback support

## 📱 Mobile Optimization

### **Responsive Breakpoints**
- **Desktop:** `> 768px` - Original XP layout, top-right positioning
- **Tablet:** `481px - 768px` - Larger touch targets, 3-column presets
- **Mobile:** `≤ 480px` - Single column layout, full-width window

### **Touch Enhancements**
- Minimum 44px touch targets
- `touch-action: none` prevents browser gestures
- Larger fonts and spacing on small screens
- Optimized button sizes for thumbs

## 🚀 Deployment

### **Static Hosting**
Perfect for deployment on:
- GitHub Pages
- Netlify
- Vercel
- Any web server with static file support

### **Integration with CRM**
1. Host the generator on your domain
2. Generate embed codes for different sections
3. Paste iframe code into your CRM's custom HTML areas
4. Backgrounds will appear behind your content

## 🎭 Windows XP Theme

The interface recreates authentic Windows XP elements:

- **Tahoma font family** - Original XP system font
- **Classic gradients** - True-to-original title bar and button styles
- **Proper borders** - Inset/outset effects matching XP
- **Color palette** - Official XP blue theme colors
- **Button behaviors** - Hover and active states

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/new-preset`
3. Commit changes: `git commit -am 'Add new preset'`
4. Push to branch: `git push origin feature/new-preset`
5. Submit a Pull Request
