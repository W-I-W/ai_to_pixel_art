# AI → Pixel Art Studio

A lightweight browser-based tool for converting AI-generated images, illustrations, portraits, backgrounds, and regular images into pixel art.

Everything runs **locally in your browser** — no server, no account, and no image upload required.

## Features

- Convert PNG, JPG, WEBP, and other browser-supported image formats to pixel art
- Drag & drop image loading
- Adjustable pixel resolution
- Adjustable color count
- Contrast control
- Saturation control
- Edge strength control
- Edge threshold control
- Transparency preservation
- Pixel-perfect PNG export
- Export scaling: x1, x2, x4, x8, x12
- English and Russian interface
- Responsive layout for desktop and smaller screens
- Multiple pixel-art processing modes
- Quick presets for characters, portraits, backgrounds, and retro graphics
- Quick preview variants

## Processing Modes

AI → Pixel Art Studio includes several ways to process an image:

### Auto Palette + Floyd–Steinberg

Automatically generates a palette from the source image and applies Floyd–Steinberg dithering.

Good for:

- detailed illustrations
- gradients
- AI-generated images
- retro-style shading

### Auto Palette without Dithering

Generates a palette automatically but keeps transitions clean and solid.

Good for:

- game characters
- sprites
- icons
- clean pixel-art assets

### Auto Palette + Bayer 4×4

Uses ordered Bayer dithering.

Good for:

- retro computer graphics
- patterned shading
- old-school game visuals

### Game Boy Palette

Converts the image using a classic four-color green palette.

### Retro 16 Colors

Uses a fixed 16-color retro palette.

### Grayscale Pixel Art

Converts the image into a limited grayscale palette.

### RGB Posterize

Reduces RGB channel levels to create harder color transitions and a stylized pixel-art look.

## Edge Controls

The application includes additional controls for emphasizing borders between color transitions.

### Edge Strength

Controls how strongly detected edges are darkened.

Higher values create more visible separation between shapes and color regions.

### Edge Threshold

Controls how different neighboring pixels must be before they are considered an edge.

- Lower value → more edges are detected
- Higher value → only strong transitions are emphasized

These settings are especially useful when converting smooth AI-generated illustrations into more readable game sprites.

## Quick Presets

Several presets are included:

- **Character** — suitable for game characters and sprites
- **Portrait** — keeps more colors and facial detail
- **Background** — uses a higher pixel resolution
- **Retro** — stronger pixel-art styling with a limited palette

All preset values can be changed manually afterward.

## How to Use

1. Open `index.html` in a modern browser.
2. Drop an image into the upload area or click it to select a file.
3. Select a processing mode.
4. Adjust:
   - pixel width
   - number of colors
   - contrast
   - saturation
   - edge strength
   - edge threshold
5. Click **Process**.
6. Choose the PNG export scale.
7. Click **Download PNG**.

No installation is required.

## Running Locally

You can simply open:

```text
index.html
```

in Chrome, Edge, Firefox, or another modern browser.

You can also run it using any simple local web server.

For example, with Python:

```bash
python -m http.server 8080
```

Then open:

```text
http://localhost:8080
```

## Deployment

Because the project is entirely client-side, it can be hosted easily on:

- GitHub Pages
- itch.io
- Netlify
- Cloudflare Pages
- Vercel
- any static web hosting

### GitHub Pages

1. Upload `index.html` to your repository.
2. Open **Settings → Pages**.
3. Select the branch containing the site.
4. Save the configuration.
5. GitHub will provide a public URL for the application.

## Privacy

Images are processed locally using the browser's Canvas API.

The application does not require images to be uploaded to a remote server.

This makes it useful for working with:

- unfinished game assets
- private artwork
- AI-generated concepts
- prototypes
- commercial project images

## Technology

The project is intentionally simple and dependency-free.

It uses:

- HTML
- CSS
- JavaScript
- Canvas API

No frameworks or external JavaScript libraries are required.

## Browser Support

Recommended:

- Google Chrome
- Microsoft Edge
- Firefox
- other modern Chromium-based browsers

JavaScript must be enabled.

## Project Structure

```text
AI-Pixel-Art-Studio/
│
├── index.html
└── README.md
```

The application is currently contained in a single `index.html` file, which makes it easy to distribute, modify, and host.

## Screenshots

You can add screenshots to your repository and reference them here:

```markdown
![AI Pixel Art Studio](screenshots/app.png)
```

Suggested structure:

```text
screenshots/
└── app.png
```

## Author

**Seitmukhametov Damir**

Developer: **Bow Pixel**

## Support the Developer

If you find this tool useful and want to support the developer, you can check out Bow Pixel applications on Steam:

[View Bow Pixel on Steam](https://store.steampowered.com/search/?hwtype=0&developer=Bow%20Pixel&ndl=1)

## Contributing

Contributions, suggestions, bug reports, and improvements are welcome.

You can:

- open an Issue
- suggest new palettes
- suggest additional dithering algorithms
- improve mobile usability
- add export formats
- improve pixel-art conversion algorithms

## Ideas for Future Versions

Possible future improvements include:

- PICO-8 palette
- NES palette
- Commodore 64 palette
- custom palette import
- custom palette editor
- before/after comparison slider
- batch image processing
- sprite sheet export
- outline color selection
- background removal
- automatic pixel-art settings
- indexed PNG export
- palette export

## License

This project is licensed under the **MIT License**.

See the [LICENSE](LICENSE) file for details.

---

Made with pixels by **Seitmukhametov Damir / Bow Pixel**.
