# Markdown to HTML Converter

This static web page converts a markdown file (input.md) to HTML using Marked.js and applies syntax highlighting to code blocks using Highlight.js.

## Features
- Converts markdown to HTML using Marked.js
- Syntax highlighting for code blocks with Highlight.js
- Tabbed interface to switch between HTML output and Markdown source
- Renders output in the #markdown-output div
- Shows raw markdown in #markdown-source div

## Libraries Used
- [Marked.js](https://marked.js.org/) - Markdown parser
- [Highlight.js](https://highlightjs.org/) - Syntax highlighting

## How It Works
1. The page fetches the input.md file
2. Shows raw markdown in the source tab
3. Uses Marked.js to convert markdown to HTML
4. Injects the HTML into the #markdown-output container
5. Applies syntax highlighting to all code blocks
6. Users can toggle between tabs to see either the rendered HTML or the original Markdown