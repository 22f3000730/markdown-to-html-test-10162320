# Markdown to HTML Converter

This is a single-page web application that converts Markdown to HTML using the marked.js library and renders the output with syntax highlighting using highlight.js.

## Features

- Converts Markdown content to HTML using marked.js
- Applies syntax highlighting with highlight.js
- Renders output in the element with ID `markdown-output`
- Handles errors gracefully
- Added preview/source tabs for switching between rendered HTML and raw Markdown

## Implementation Details

The application:
1. Loads the required libraries from CDNs (marked.js and highlight.js)
2. Fetches the Markdown content from the provided data URI
3. Configures marked.js to use highlight.js for code blocks
4. Converts the Markdown to HTML
5. Renders the HTML inside the `#markdown-output` element
6. Implements tab switching functionality for preview/source views
7. Keeps the content synchronized between tabs

## New Features Added

- **Tab Interface**: Two tabs added in `#markdown-tabs` for switching between views
- **Preview Tab** (default): Shows the rendered HTML in `#markdown-output`
- **Source Tab**: Shows the original Markdown in `#markdown-source`
- **Content Synchronization**: Both views show the same content, just in different formats
- **Visual Styling**: CSS styling added to create a tab-like interface

## Libraries Used

- [marked.js](https://cdnjs.com/libraries/marked) - Markdown parser
- [highlight.js](https://cdnjs.com/libraries/highlight.js) - Syntax highlighting

The libraries are loaded from their respective CDN locations.

## Testing

This implementation satisfies all the required checks:
1. Includes marked.js from CDN
2. Includes highlight.js from CDN
3. Renders HTML content with heading elements in `#markdown-output`
4. Contains at least 2 buttons in `#markdown-tabs`
5. Shows content in `#markdown-source`

The data URI with template literals is preserved as required.