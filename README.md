# HTML Table Parser

A lightweight Python command-line tool that extracts the first HTML table from a local file or web page and exports it as `output.csv`.

## Overview

This project demonstrates a simple, dependency-free approach to parsing HTML tables with Python's standard library. It accepts either a local HTML file path or an HTTP/HTTPS URL, reads the page content, parses table rows and cells, and writes the first discovered table to a CSV file.

## Features

- Reads HTML from a local file or a web URL
- Parses `<table>`, `<tr>`, `<td>`, and `<th>` elements
- Exports the first table to `output.csv`
- Uses only Python standard library modules
- Includes a browser-like user agent for web requests

## Tech Stack

- Python
- `html.parser`
- `urllib.request`
- `csv`

## Getting Started

### Requirements

- Python 3.8 or newer

### Run the Parser

```bash
python read_html_table.py <URL-or-file-path>
```

Example with a web page:

```bash
python read_html_table.py https://example.com/page-with-table.html
```

Example with a local file:

```bash
python read_html_table.py sample.html
```

After a successful run, the parsed table is written to:

```text
output.csv
```

## Project Structure

```text
html-table-parser/
├── read_html_table.py   # HTML table parser and CLI entry point
├── output.csv           # Example/generated CSV output
└── README.md
```

## Future Improvements

- Add an option to choose which table to export
- Support output file names from the command line
- Preserve spacing inside complex table cells
- Add automated tests with sample HTML fixtures

## Author

Sandeep Shah
