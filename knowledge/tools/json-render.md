# json-render

**Repo:** https://github.com/vercel-labs/json-render

A library for AI-generated interfaces that constrains AI to predefined components through JSON schemas.

## What It Does

json-render enables fully generative interfaces by:
- Providing a **constrained vocabulary** to AI (only components you define)
- Generating **predictable JSON output** that always matches your schema
- **Streaming** and rendering progressively as the model responds

## Key Features

- **Guardrailed** - AI can only use components in your catalog
- **Predictable** - JSON output matches your schema every time
- **Fast** - Progressive rendering as model responds
- **TypeScript** - Built with Zod for schema validation

## Packages

- `@json-render/core` - Types, schemas, visibility, actions, validation
- `@json-render/react` - React renderer, providers, hooks

## Use Cases

- User-generated dashboards from prompts
- AI-generated widgets and data visualizations
- Safe component catalog generation
- Progressive UI streaming

## Tech Stack

- TypeScript
- React
- Zod (schema validation)
- Streaming JSON
