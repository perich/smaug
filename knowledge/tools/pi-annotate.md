# Pi Annotate

**Repository:** https://github.com/nicobailon/pi-annotate
**Author:** nicobailon
**Language:** JavaScript
**Stars:** 36

## Overview

Pi Annotate is a Chrome extension and Pi extension system that provides visual annotation capabilities for AI agents. It enables a Figma-like annotation experience where users can click on web elements, add comments, and have the agent receive comprehensive context including selectors, CSS, box model, accessibility info, and screenshots.

## Key Features

- **Visual Element Selection**: DevTools-like element picker in vanilla JavaScript
- **Inline Note Cards**: Draggable floating cards with per-element comments, SVG connectors linking notes to elements
- **Context Capture**: Automatic capture of box model (padding, border, margin), accessibility information (role, name, focusable, ARIA states), HTML attributes, and CSS styles
- **Screenshots**: Individual crops per element or full-page mode with numbered badges identifying elements
- **Debug Mode**: Computed styles (40+ properties), parent context, and CSS variables
- **Restricted Tab Handling**: Auto-injection on fresh tabs and URL routing for chrome:// restrictions

## Architecture

The system uses a Unix socket bridge connecting:
- **Pi Extension** (TypeScript) - `/annotate` command and tool
- **Chrome Extension** (vanilla JS) - Content script and background worker
- **Native Host** (Node.js) - Socket/native messaging bridge

## Usage

```bash
/annotate                  # Annotate current Chrome tab
/annotate https://x.com    # Open URL first, then annotate
```

### Controls

| Action | How |
|--------|-----|
| Select element | Click on page |
| Cycle ancestors | Alt/⌥+scroll while hovering |
| Multi-select | Toggle "Multi" or Shift+click |
| Add comment | Type in note card textarea |
| Toggle screenshot | 📷 button in note card header |
| Expand/collapse all | ▼/▲ buttons in toolbar |
| Toggle annotation UI | ⌘/Ctrl+Shift+P |
| Close | ESC |

## Output Format

The annotation output is delivered in markdown format with detailed element information:

```markdown
## Page Annotation: https://example.com
**Viewport:** 1440×900
**Context:** [User comment]

### Selected Elements (N)

1. **tag**
   - Selector: `#id`
   - Classes: `class1, class2`
   - Text: "content"
   - **Box Model:** dimensions (content, padding, border, margin)
   - **Attributes:** attribute="value"
   - **Styles:** key CSS properties
   - **Accessibility:** role, name, focusable state
   - **Comment:** User's note
```

## Topics

- ai-tools
- annotation
- chrome-extension
- pi

## Setup

1. Install Pi Extension: `pi install npm:pi-annotate`
2. Load Chrome Extension: Enable Developer mode at `chrome://extensions`, click Load unpacked, select `chrome-extension/` folder
3. Install Native Host: Run `./install.sh <extension-id>` from `chrome-extension/native/`

## Security

- Auth token generated per-run at `/tmp/pi-annotate.token`
- Socket and token files use 0600 permissions for access control
