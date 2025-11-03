# JSON to Table Converter

A lightweight, client-side web tool to convert and visualize JSON data as interactive, searchable tables with advanced export capabilities.

![Version](https://img.shields.io/badge/version-2.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Responsive](https://img.shields.io/badge/responsive-yes-success)

## ✨ Features

- **Smart JSON Handling**: Automatically processes arrays, objects, and nested structures
- **Expandable Cells**: Click to expand long JSON arrays/objects for better readability
- **Fully Responsive**: Optimized for desktop, tablet, and mobile devices
- **Multiple Input Methods**: Paste JSON, upload files, or load from URLs
- **Advanced Table Features** (powered by DataTables):
  - Search and filter
  - Column sorting
  - Pagination
  - Export to CSV, Excel, PDF
  - Copy to clipboard
  - Print functionality
  - Column visibility toggle
  - Row selection
- **XSS Protection**: All inputs sanitized for safe public use
- **Dark Mode**: Toggle between light and dark themes
- **History**: Saves your last 10 conversions locally
- **Statistics**: View record counts and numeric summaries
- **Zero Installation**: Single HTML file, works offline

## 🚀 Live Demo

**Try it now:** [https://ckraheem.github.io/json-to-table](https://ckraheem.github.io/json-to-table)

## 📖 Usage

### Quick Start

1. Visit the live demo or open `index.html` in your browser
2. Paste your JSON data (supports any valid JSON format)
3. Click "Convert to Table"
4. Use the toolbar to search, filter, sort, or export your data

### Supported JSON Formats

```json
// Array of objects
[
  {"id": 1, "name": "John", "age": 30},
  {"id": 2, "name": "Jane", "age": 25}
]

// Single object (auto-wrapped)
{"id": 1, "name": "John", "age": 30}

// Object with array property (auto-detected)
{
  "users": [
    {"id": 1, "name": "John"},
    {"id": 2, "name": "Jane"}
  ]
}

// Nested objects (auto-flattened to dot notation)
[
  {
    "name": "John",
    "address": {"city": "NYC", "zip": "10001"}
  }
]
```

### Complex Data Handling

For arrays or objects longer than 100 characters, the tool displays a preview with an expand button. Click to view the full formatted JSON.

## ⚙️ Configuration

Access settings via the **Settings** tab:

- **Auto-flatten nested objects**: Converts nested objects to dot notation columns
- **Show row numbers**: Adds a numbered column
- **Show table statistics**: Displays record counts and numeric summaries
- **Pretty-print complex data**: Formats arrays/objects with indentation
- **Save conversions to history**: Keeps last 10 conversions in browser storage

## 🚀 Deployment

### Deploy to GitHub Pages

1. **Create a new repository** on GitHub
   - Make it public
   - Don't initialize with README

2. **Push your code**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/json-table.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` / `(root)`
   - Save

4. **Access your site**
   - Visit: `https://yourusername.github.io/json-table`

### Self-Hosting

Simply upload `index.html` to any web server. No build process or dependencies required.

## 🛠️ Technologies

- **Bootstrap 5**: Responsive UI framework
- **DataTables**: Advanced table features
- **jQuery**: DOM manipulation (required by DataTables)
- **Vanilla JavaScript**: Core functionality

## 📝 License

MIT License - Free for personal and commercial use.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

## 📧 Support

For questions or issues, please [open an issue](https://github.com/ckraheem/json-table/issues) on GitHub.

---

**Made with ❤️ by the community**
