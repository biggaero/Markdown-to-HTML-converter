# Markdown to HTML Converter

A Python script that converts Markdown files to beautifully styled HTML documents with professional formatting and responsive design.

## Features

- ✅ Convert Markdown files to HTML with professional styling
- ✅ Support for tables, fenced code blocks, and table of contents
- ✅ Responsive design that works on desktop and mobile
- ✅ Clean, modern styling with proper typography
- ✅ Syntax highlighting for code blocks
- ✅ Automatic output filename generation
- ✅ Custom output filename support
- ✅ UTF-8 encoding support

## Requirements

- Python 3.x
- `markdown` library

### Installation

Install the required dependency:

```bash
pip install markdown
```

## Usage

### Basic Usage

Convert a Markdown file to HTML (output file will have the same name with `.html` extension):

```bash
python md_to_html.py document.md
```

### Custom Output File

Specify a custom output filename:

```bash
python md_to_html.py document.md output.html
```

### Make Script Executable (Optional)

On Unix-like systems, you can make the script executable:

```bash
chmod +x md_to_html.py
./md_to_html.py document.md
```

## Supported Markdown Extensions

The script supports the following Markdown extensions:

- **Tables**: Create formatted tables with borders and styling
- **Fenced Code Blocks**: Code blocks with language specification
- **Table of Contents**: Automatic TOC generation from headings

## Output Styling

The generated HTML includes professional styling with:

- Modern, clean typography using system fonts
- Responsive design (max-width: 1000px, centered)
- Styled headings with underlines
- Syntax-highlighted code blocks with background
- Bordered tables with alternating row colors
- Styled blockquotes with left border
- Professional color scheme using blues and grays

## Examples

### Example 1: Basic Conversion
```bash
python md_to_html.py README.md
# Creates: README.html
```

### Example 2: Custom Output
```bash
python md_to_html.py documentation.md docs.html
# Creates: docs.html
```

### Example 3: Multiple Files
```bash
python md_to_html.py chapter1.md
python md_to_html.py chapter2.md
python md_to_html.py chapter3.md
# Creates: chapter1.html, chapter2.html, chapter3.html
```

## Error Handling

The script includes robust error handling:

- Checks if input file exists
- Provides clear error messages
- Returns appropriate exit codes
- Handles UTF-8 encoding properly

## File Structure

```
md_to_html.py          # Main script
README.md             # This documentation
example.md            # (Your markdown files)
example.html          # (Generated HTML files)
```

## Function Reference

### `convert_md_to_html(md_file, output_file=None)`

Converts a Markdown file to HTML.

**Parameters:**
- `md_file` (str): Path to the input Markdown file
- `output_file` (str, optional): Path to the output HTML file. If not provided, uses the same name as input with `.html` extension

**Returns:**
- `bool`: True if conversion successful, False otherwise

## CSS Styling Details

The generated HTML includes embedded CSS with:

- **Typography**: System font stack with fallbacks
- **Layout**: Centered content with maximum width
- **Colors**: Professional blue and gray color scheme
- **Code**: Monospace font with background highlighting
- **Tables**: Bordered with header styling
- **Links**: Blue color with hover effects

## License

This script is provided as-is for educational and practical use. Feel free to modify and distribute according to your needs.

## Contributing

To contribute improvements:

1. Test your changes with various Markdown files
2. Ensure UTF-8 encoding is preserved
3. Maintain the existing styling consistency
4. Add error handling for edge cases

## Troubleshooting

### Common Issues

**Issue**: `ModuleNotFoundError: No module named 'markdown'`
**Solution**: Install the markdown library: `pip install markdown`

**Issue**: `Error: File 'filename.md' not found.`
**Solution**: Check the file path and ensure the file exists

**Issue**: Permission denied when writing output file
**Solution**: Ensure you have write permissions in the output directory

### Getting Help

If you encounter issues:
1. Check that the input file exists and is readable
2. Verify you have write permissions for the output location
3. Ensure the `markdown` library is installed
4. Check that you're using Python 3.x

## Version Information

- Script Version: 1.0
- Python Version: 3.x required
- Dependencies: markdown library
