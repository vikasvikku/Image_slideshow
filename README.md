# Image Slideshow

A fullscreen image slideshow application that automatically cycles through images with smooth transitions.

## Features

- **Automatic slideshow**: Images change every 5 seconds
- **Smooth transitions**: 1-second fade effect between images
- **Fullscreen display**: Images fill the entire screen
- **Colossal image support**: Properly scales large images while maintaining aspect ratio
- **Image preloading**: All images load before slideshow starts
- **Loading indicator**: Shows progress while images are being prepared
- **Continuous loop**: Slideshow runs indefinitely

## Project Structure

```
Image_slideshow/
├── index.html          # Main slideshow file
├── Images/             # Image folder containing 21 PNG files
│   ├── Segment_B_miss.png
│   ├── Segment_A_miss.png
│   ├── Earth_icon_missing.png
│   └── ... (18 more images)
└── README.md           # This file
```

## How to Run

### Method 1: Double-click
1. Navigate to the `Image_slideshow` folder
2. Double-click `index.html`
3. Slideshow opens in your default browser

### Method 2: Browser open
1. Open any web browser
2. Press `Ctrl + O` or go to File → Open
3. Select `index.html`

### Method 3: Drag and drop
1. Open a web browser
2. Drag `index.html` into the browser window

## Technical Details

- **No dependencies**: Pure HTML, CSS, and JavaScript
- **Browser compatibility**: Works in all modern browsers
- **Responsive design**: Adapts to any screen size
- **Image format**: Supports PNG images
- **Performance optimized**: Images are preloaded for smooth playback

## Updates Made

### Original Issues Fixed:
- ❌ Used absolute Windows file paths (wouldn't work in browser)
- ❌ Only included 4 images
- ❌ Basic styling without proper image scaling

### Improvements Added:
- ✅ **Relative paths**: Uses `Images/` folder structure
- ✅ **All images included**: Now displays all 21 images from the folder
- ✅ **Colossal image support**: `object-fit: contain` properly scales large images
- ✅ **Image preloading**: Prevents delays during slideshow
- ✅ **Loading indicator**: User feedback while images load
- ✅ **Error handling**: Continues if some images fail to load
- ✅ **Smooth transitions**: Professional fade effects
- ✅ **Fullscreen optimization**: Perfect for presentations

## Customization

### Change slide duration:
Edit line 159 in `index.html`:
```javascript
setInterval(nextSlide, 5000); // 5000 = 5 seconds
```

### Add more images:
1. Place images in the `Images/` folder
2. Add image paths to the `images` array in `index.html`

### Modify transition speed:
Edit the CSS transition duration:
```css
transition: opacity 1s ease-in-out; /* 1s = 1 second */
```

## Requirements

- Any modern web browser (Chrome, Firefox, Edge, Safari)
- No internet connection required
- No additional software installation needed