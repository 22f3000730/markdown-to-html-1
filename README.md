# Markdown to HTML Converter

This static web page converts a markdown file to HTML using Marked.js and applies syntax highlighting to code blocks using Highlight.js.

## Features
- Converts markdown to HTML using Marked.js
- Syntax highlighting for code blocks with Highlight.js
- Tabbed interface to switch between HTML output and Markdown source
- Renders output in the #markdown-output div
- Shows raw markdown in #markdown-source div
- Displays a live word count badge #markdown-word-count that updates after every render
- Word count is formatted with Intl.NumberFormat
- Shows active source in #markdown-source-label
- Supports loading Markdown from a ?url= parameter when present

## Libraries Used
- [Marked.js](https://marked.js.org/) - Markdown parser
- [Highlight.js](https://highlightjs.org/) - Syntax highlighting

## How It Works
1. The page checks for a ?url= parameter
2. If present, loads markdown from that URL
3. Otherwise, loads from the embedded base64 data URI
4. Shows raw markdown in the source tab
5. Uses Marked.js to convert markdown to HTML
6. Injects the HTML into the #markdown-output container
7. Applies syntax highlighting to all code blocks
8. Users can toggle between tabs to see either the rendered HTML or the original Markdown
9. Word count is calculated and displayed in formatted form in #markdown-word-count
10. Active source is shown in #markdown-source-label

## Implementation Details
- The word count considers words as non-whitespace sequences separated by whitespace
- The count is formatted with locale-appropriate thousands separators using Intl.NumberFormat
- The badge updates every time new markdown content is rendered
- Template literals like `${...}` within data URIs are preserved as-is without decoding
- When ?url= parameter is present, it takes precedence over the embedded content

## Example Usage

### Default mode
Simply open the page to view the embedded markdown content

### URL parameter mode
Open the page with a URL parameter: `?url=https://example.com/sample.md`

The application will load and render the content from that URL instead of the embedded content.