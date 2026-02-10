# stooru
A simple static tag-based image gallery heavily inspired by booru image boards

## File Structure

```
your-gallery/
├── index.html          # Main HTML file
├── data.json           # Image metadata and tags
├── images/             # Directory for your images
│   ├── image001.jpg
│   ├── image002.jpg
│   └── ...
└── README.md          # This file
```

## Setup Instructions

1. **Clone this repo:**
   ```bash
   git clone https://github.com/zuiraito/stooru.git
   ```

2. **Add your images:**
   - Place all your images in the `images/` directory
   - Supported formats: jpg, jpeg, png, gif, webp (todo: video formats)

3. **Linking images and adding Tags:**
   Open the `data.json` file.
   Entry Template:
   ```json
   {
     "id": 1,
     "filename": "my-photo.jpg",
     "title": "Beautiful Sunset",
     "tags": ["landscape", "sunset", "nature"]
   }
   ```
   Optionally add a text block:
   ```json
     "text": "A short story about the image",
   ```
6. **Preview:**
  - Preview before deplying using `python -m http.server 8000` and opening `http://127.0.0.1:8000/` in a webbrowser.

## Deployment

This is a static site, so you can host it anywhere:
- GitHub Pages
- Netlify
- Vercel
- Any web hosting service
- Just upload all files including the images directory

## TODOs
- [ ] Add support for videos
