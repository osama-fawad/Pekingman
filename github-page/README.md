# Pekingman GitHub Pages Site

This folder is the publishable static site for the Pekingman project.

## Contents

- `index.html` - page markup
- `styles.css` - page styling
- `media/pekingman-demo.mp4` - web-optimized copy of `../demo_video/北京猿人.mp4`
- `media/poster.jpg` - poster frame generated from the demo video

## Local Preview

From this folder:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## GitHub Pages Publishing

Create a GitHub repository using only the contents of this folder, then enable Pages from the repository's `main` branch root.
