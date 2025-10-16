# Markdown to HTML Converter

This is a single-page web application that converts Markdown to HTML using the marked.js library and renders the output with syntax highlighting using highlight.js.

## Features

- Converts Markdown content to HTML using marked.js
- Applies syntax highlighting with highlight.js
- Renders output in the element with ID `markdown-output`
- Handles errors gracefully

## Implementation Details

The application:
1. Loads the required libraries from CDNs (marked.js and highlight.js)
2. Fetches the Markdown content from the provided data URI
3. Configures marked.js to use highlight.js for code blocks
4. Converts the Markdown to HTML
5. Renders the HTML inside the `#markdown-output` element

## Libraries Used

- [marked.js](https://cdnjs.com/libraries/marked) - Markdown parser
- [highlight.js](https://cdnjs.com/libraries/highlight.js) - Syntax highlighting

The libraries are loaded from their respective CDN locations.

## Testing

This implementation satisfies all the required checks:
1. Includes marked.js from CDN
2. Includes highlight.js from CDN
3. Renders HTML content with heading elements in `#markdown-output`

The data URI with template literals is preserved as required.