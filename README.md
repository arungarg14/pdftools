# 📄 PDFForge — Your Free PDF Toolkit

> A powerful, privacy-first PDF utility suite that runs entirely in your browser. No uploads, no servers, no sign-ups — just fast, free PDF tools at your fingertips.

---

## 🌟 Overview

PDFForge is a client-side web application that provides a comprehensive set of PDF manipulation tools. Built with a dark, modern UI and inspired by the best PDF tooling on the web, it lets users merge, split, rotate, compress, watermark, and convert PDFs — all without their files ever leaving their device.

The app is split into two sections:
- **Live Tools** — fully functional, runs 100% in the browser
- **Coming Soon** — server-powered tools currently in development

---

## ✅ Live Tools (Client-Side)

| Tool | Description |
|---|---|
| 🔗 Merge PDF | Combine multiple PDFs into one, with drag-to-reorder support |
| ✂️ Split PDF | Split by all pages, custom page range, or every N pages |
| 🔄 Rotate PDF | Rotate all, odd, or even pages by 90°, 180°, or 270° |
| 🖼️ Image to PDF | Convert JPG, PNG, WebP images to PDF with page size & orientation options |
| 🖼️ PDF to Image | Extract PDF pages as downloadable PNG images |
| 💧 Add Watermark | Stamp custom text with configurable color, opacity, size, and rotation |
| 🔢 Page Numbers | Add page numbers with custom position, prefix, and start number |
| 🗜️ Compress PDF | Reduce PDF file size by optimising object streams |
| 🔓 Unlock PDF | Remove password protection from PDFs (password required) |

---

## 🚀 Coming Soon (Server-Side)

These tools require backend infrastructure and are currently in development:

| Tool | Reason |
|---|---|
| 📝 Word ↔ PDF | Requires LibreOffice / MS Word rendering engine |
| 📊 Excel ↔ PDF | Requires spreadsheet layout engine |
| 📑 PowerPoint ↔ PDF | Requires slide rendering engine |
| 🔐 Protect PDF | Requires Ghostscript / qpdf for encryption |
| 🔍 OCR PDF | Requires Tesseract or a cloud OCR API |
| 🌐 HTML to PDF | Requires headless browser (Puppeteer / Playwright) |
| 🔏 Sign PDF | Requires PKI certificate infrastructure |
| ⬛ Redact PDF | Requires deep PDF object manipulation |
| 🤖 AI Summarizer | Requires LLM API integration |

---

## 🛠️ Tech Stack

### Frontend
- **HTML5** — semantic markup, single-file architecture
- **CSS3** — custom properties (CSS variables), CSS Grid, Flexbox, transitions & animations
- **Vanilla JavaScript (ES2020+)** — no frameworks, async/await, FileReader API, Blob & URL APIs

### PDF Processing
- **[pdf-lib](https://pdf-lib.js.org/) v1.17.1** — core PDF manipulation library (merge, split, rotate, watermark, page numbers, compress, unlock)
- **Canvas API** — used for PDF-to-image page rendering

### File Handling
- **FileReader API** — reads local files as ArrayBuffer for PDF processing
- **Drag & Drop API** — drag-and-drop file input on drop zones
- **Blob + URL.createObjectURL** — generates downloadable output files client-side

### Design
- **Custom dark theme** — space-dark background (`#0d1117`) with teal (`#00c9a7`) and amber (`#f0a500`) accents
- **CSS Grid** — responsive tool card layout
- **No external CSS frameworks** — fully hand-crafted styles

### Hosting
- Any static file host — **no backend required** for live tools
- Recommended: [Vercel](https://vercel.com), [Netlify](https://netlify.com), [GitHub Pages](https://pages.github.com)

---

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/your-username/pdfforge.git

# Navigate into the project
cd pdfforge

# Open directly in browser (no build step needed)
open index.html
```

Or simply deploy the `index.html` to any static hosting provider.

---

## 🔒 Privacy

PDFForge processes all files **locally in your browser**. Your documents are never uploaded to any server, never stored, and never transmitted over the network. All processing happens in-memory and files are discarded when you close the tab.

---

## 📁 Project Structure

```
pdfforge/
├── index.html       # Entire application (single-file)
└── README.md        # This file
```

---

## 🤝 Contributing

Contributions are welcome! If you'd like to add a new client-side tool or improve existing ones:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/my-tool`)
3. Commit your changes (`git commit -m 'Add my tool'`)
4. Push to the branch (`git push origin feature/my-tool`)
5. Open a Pull Request

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

<p align="center">Built with ❤️ — no servers harmed in the making of this app.</p>
