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

### Quick Start (Single File Method)

The easiest way to use this tool without installing git or command-line tools:

1.  **Download the Source Code**
    - Navigate to the source code file in this repository (e.g., `src/offline_pdf_arranger`).
    - Click the **"Raw"** button (or right-click the "Raw" button and choose "Save Link As...").

2.  **Prepare the File**
    - Save the file to your computer.
    - Rename the file so it ends with the **`.html`** extension (e.g., rename `offline_pdf_arranger` to `offline_pdf_arranger.html`).

3.  **Run in Browser**
    - Drag and drop the `.html` file directly into any Chromium-based browser tab (Google Chrome, Microsoft Edge, Brave, etc.).
    - Alternatively, right-click the file and select "Open with" > "Google Chrome".

### Developer Setup (Git Clone)

If you are a developer and want to contribute or modify the code:

1.  **Clone the repository**
    ```bash
    git clone [https://github.com/yourusername/offline-pdf-arranger.git](https://github.com/yourusername/offline-pdf-arranger.git)
    cd offline-pdf-arranger
    ```

2.  **Open the application**
    ```bash
    # Open the HTML file directly
    open src/offline_pdf_arranger.html  # macOS
    xdg-open src/offline_pdf_arranger.html  # Linux
    start src/offline_pdf_arranger.html  # Windows
    ```

### Using a Local Server (Optional)

If you prefer to run it through a local web server (recommended for development):

```bash
# Using Python 3
python3 -m http.server 8000

# Using Node.js built-in
node --eval "require('http').createServer((req, res) => require('fs').createReadStream(req.url.slice(1)).pipe(res)).listen(8000)"
