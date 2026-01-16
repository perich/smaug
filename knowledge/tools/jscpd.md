# jscpd

**Author:** kucherenko
**GitHub:** https://github.com/kucherenko/jscpd
**Stars:** 5,193
**Language:** TypeScript

A copy/paste detector for programming source code supporting 150+ formats, implementing the Rabin-Karp algorithm for efficient duplication detection.

## Overview

Copy/paste is a common technical debt in projects. jscpd finds duplicated blocks implemented in 150+ programming languages and digital document formats.

## Installation

```bash
npm install -g jscpd
```

## Usage

```bash
npx jscpd /path/to/source
jscpd /path/to/code
jscpd --pattern "src/**/*.js"
```

## Features

- Supports 150+ programming languages and document formats
- Implements Rabin-Karp algorithm for efficient duplicate detection
- Multiple output reporters (HTML, badge, etc.)
- Can be used as CLI or programmatic API
- Server mode available for integration

## Packages

| Package | Description |
|---------|-------------|
| jscpd | Main CLI and API |
| jscpd-server | Standalone server application |
| @jscpd/core | Core detection algorithm |
| @jscpd/finder | File duplication detector |
| @jscpd/tokenizer | Source code tokenizer |
| @jscpd/leveldb-store | LevelDB store for large repos |
| @jscpd/html-reporter | HTML report generation |
| @jscpd/badge-reporter | Badge report generation |

## JSCPD Server

Start server and check code for duplication:

```bash
jscpd-server
curl -X POST http://localhost:3000/api/check \
  -H "Content-Type: application/json" \
  -d '{
    "code": "console.log(\"hello\");\nconsole.log(\"world\");",
    "format": "javascript"
  }'
```

## Programming API

```typescript
import {IClone} from '@jscpd/core';
import {jscpd} from 'jscpd';

const clones: Promise<IClone[]> = jscpd(process.argv);
```

## Tags
[[code-quality]] [[duplication-detection]] [[developer-tools]] [[linting]] [[typescript]]
