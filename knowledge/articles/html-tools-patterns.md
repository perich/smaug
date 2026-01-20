# Useful Patterns for Building HTML Tools

## Overview
Simon Willison's comprehensive guide on building single-file HTML tools that combine HTML, JavaScript, and CSS into standalone applications. Over 150 tools have been built using these patterns.

## HTML Tool Definition
A single HTML file containing:
- Inline HTML markup
- Inline JavaScript logic
- Inline CSS styling
- No build process required
- Can be copy-pasted from LLM responses

## Key Principles
1. **Single file**: Minimizes hosting hassle and enables easy distribution
2. **No React or build steps**: Avoids JSX compilation overhead
3. **CDN dependencies**: Load libraries from CDNs when needed
4. **Keep small**: A few hundred lines for maintainability

## Tools Collection
- **svg-render**: Convert SVG code to downloadable JPEGs/PNGs
- **pypi-changelog**: Generate diffs between PyPI package releases
- **bluesky-thread**: Nested view of Bluesky discussion threads
- **And 150+ more**: Browse at https://tools.simonwillison.net/

## Core Patterns

### Prototyping
- Use Claude Artifacts, ChatGPT Canvas, or Gemini Canvas for initial development
- Prompt: "Build a canvas/artifact that..." with "No React"

### State Management
- **URL persistence**: Store application state in query parameters
- **localStorage**: For secrets and larger state objects
- Both enable stateless deployment

### Data Handling
- **File input**: Use HTML file APIs for user file uploads
- **Downloadable files**: Generate and offer files for download
- **Clipboard**: Leverage copy-paste for input/output

### Capabilities
- **CORS-enabled APIs**: Call APIs directly from the browser
- **LLM APIs**: Can be called directly via CORS from client code
- **Pyodide**: Run Python code in the browser
- **WebAssembly**: Additional possibilities for complex computations

### Debugging & Distribution
- **Debugging tools**: Build tools to debug other tools
- **Remix existing tools**: Build on previous work
- **Record prompts**: Document the prompt and transcript used
- **GitHub hosting**: Easy deployment and version control

## Deployment
- Host on GitHub Pages
- GitHub Releases for standalone HTML files
- No server required
- Single file = easy to distribute

## Resources
- **Collection**: https://tools.simonwillison.net/
- **By month view**: https://tools.simonwillison.net/by-month
- **View source**: GitHub links in tool footers
- **Prompts**: Available in commit messages and transcripts

## Author
[Simon Willison](https://simonwillison.net/)

## Published
December 10, 2025

## URL
https://simonwillison.net/2025/Dec/10/html-tools/
