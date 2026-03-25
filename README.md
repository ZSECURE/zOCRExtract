# zOCRExtract

A beautiful, 100% client-side OCR web app — extract text from images directly in your browser.  
No server required. No data ever leaves your device.

## ✨ Features

| Feature | Detail |
|---|---|
| **Drag & drop upload** | Drop one or many images onto the upload zone, or click to browse |
| **Multiple images** | Process a batch of images in a single click |
| **In-browser OCR** | Powered by [Tesseract.js](https://github.com/naptha/tesseract.js) — runs entirely client-side |
| **Copy to clipboard** | Per-image or copy-all button |
| **Download as `.txt`** | Per-image or download-all button |
| **Advanced filters** | Word-length range, starts-with / ends-with / contains, custom regex |
| **Re-apply filters** | Change filter settings after OCR without re-processing |
| **Pretty UI** | Colourful gradient dark theme, animated progress bar, responsive layout |

## 🚀 Live Demo

Once deployed, open:
```
https://<your-github-username>.github.io/zOCRExtract/
```

## 🏗️ Deploy (GitHub Pages)

1. Push code to the `main` branch.
2. In your repository go to **Settings → Pages**.
3. Under **Source** select **GitHub Actions**.
4. The workflow in `.github/workflows/deploy.yml` will automatically build and publish on every push to `main`.

## 🖥️ Run Locally

No build step required — just open `index.html` in any modern browser:

```bash
# Option 1 – open directly
open index.html          # macOS
xdg-open index.html      # Linux

# Option 2 – simple HTTP server (avoids any CORS edge-cases)
python -m http.server 8080
# then visit http://localhost:8080
```

## 🔒 Privacy

All processing happens in your browser using WebAssembly.  
Images and extracted text are **never uploaded** to any external service.

## 📄 License

MIT
