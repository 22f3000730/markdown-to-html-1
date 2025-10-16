# Markdown to HTML Converter

This static web page converts a markdown file (input.md) to HTML using Marked.js and applies syntax highlighting to code blocks using Highlight.js.

## Features
- Converts markdown to HTML using Marked.js
- Syntax highlighting for code blocks with Highlight.js
- Renders output in the #markdown-output div

## Libraries Used
- [Marked.js](https://marked.js.org/) - Markdown parser
- [Highlight.js](https://highlightjs.org/) - Syntax highlighting

## How It Works
1. The page fetches the input.md file
2. Uses Marked.js to convert markdown to HTML
3. Injects the HTML into the #markdown-output container
4. Applies syntax highlighting to all code blocks