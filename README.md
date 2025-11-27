# Offline PDF Arranger

A lightweight, client-side web application for organizing and rearranging PDF pages without uploading to any server. All processing happens locally in your browser.

## Features

- 📄 **Upload PDF files** - Select and load any PDF from your device
- 🔄 **Drag-and-drop reordering** - Easily rearrange pages by dragging them
- 👁️ **Page preview** - View all pages with thumbnail previews
- 📊 **Batch operations** - Delete or reorder multiple pages at once
- 💾 **Download modified PDF** - Export your organized PDF back to your device
- 🔒 **100% offline** - No data is sent to any server; all processing is done locally
- ⚡ **Fast and responsive** - Optimized for smooth performance

## How to Run

### Quick Start

1. **Clone or download this repository**
   ```bash
   git clone https://github.com/yourusername/offline-pdf-arranger.git
   cd offline-pdf-arranger
   ```

2. **Open the application**
   - Simply open `src/offline_pdf_arranger` file in your web browser
   - Or double-click the HTML file directly
   - Alternatively, you can open it via command line:
     ```bash
     open src/offline_pdf_arranger  # macOS
     xdg-open src/offline_pdf_arranger  # Linux
     start src/offline_pdf_arranger  # Windows
     ```

3. **Use the application**
   - Click "Upload PDF" or drag-and-drop a PDF file
   - Rearrange pages by dragging them to new positions
   - Delete unwanted pages
   - Click "Download PDF" to save your modified document

### Using a Local Server (Optional)

If you prefer to run it through a local web server:

```bash
# Using Python 3
python3 -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Using Node.js built-in
node --eval "require('http').createServer((req, res) => require('fs').createReadStream(req.url.slice(1)).pipe(res)).listen(8000)"
```

Then open `http://localhost:8000/src/offline_pdf_arranger` in your browser.

## Requirements

- Modern web browser (Chrome, Firefox, Safari, Edge)
- No additional software or dependencies required
- Works offline (except for loading the application itself)

## Browser Compatibility

- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

## Technologies Used

- **HTML5** - Structure
- **Tailwind CSS** - Styling (via CDN)
- **Font Awesome** - Icons
- **PDF.js** - PDF rendering and manipulation
- **Vanilla JavaScript** - Drag-and-drop functionality and PDF processing
- **SortableJS** - Drag-and-drop list reordering

## Usage Tips

1. **Organizing Large PDFs** - The application handles PDFs with hundreds of pages efficiently
2. **Memory Considerations** - Very large PDFs (1000+ pages) may require more RAM
3. **Supported Formats** - Works with standard PDF files; encrypted PDFs may not be supported
4. **Batch Operations** - Select multiple pages and delete them at once for efficiency

## Privacy

Your PDFs never leave your computer. All processing is done locally in your browser. No files are uploaded to any server.

## License

This project is open source and available under the MIT License.

## Contributing

Contributions are welcome! Feel free to fork the repository and submit pull requests for any improvements.

## Troubleshooting

### PDF not loading
- Ensure the file is a valid PDF
- Try a different PDF to test
- Check browser console for error messages

### Drag-and-drop not working
- Ensure you're using a modern browser
- Try refreshing the page
- Check that JavaScript is enabled

### Download not working
- Check your browser's download settings
- Ensure you have sufficient disk space
- Try a different browser

## Author

Created as a utility for offline PDF document management.

---

For more information or issues, please create an issue in the repository.
