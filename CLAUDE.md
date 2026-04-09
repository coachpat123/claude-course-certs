# CLAUDE.md

## Project Overview
**uigen** is a Next.js 15 UI generation app powered by Claude AI. It uses the AI SDK to generate React components via chat interface.

## Tech Stack
- **Framework**: Next.js 15 (App Router, Turbopack)
- **Language**: TypeScript
- **AI**: Anthropic Claude via `@ai-sdk/anthropic`
- **Database**: Prisma ORM
- **UI**: Radix UI + Tailwind CSS v4
- **Editor**: Monaco Editor
- **Testing**: Vitest + React Testing Library

## Key Commands
```bash
npm run dev       # start dev server (port 3000)
npm run build     # production build
npm run test      # run Vitest tests
npm run setup     # install deps + run DB migrations
npm run db:reset  # reset database
```

## Code Conventions
- Use `@/` absolute imports
- Components live in `src/` with App Router structure
- Tests go in `__tests__/` directories next to source files
- Use Radix UI primitives + Tailwind for all UI components

## PR Review Guidelines
- Check for type safety and proper TypeScript usage
- Verify AI SDK usage follows streaming patterns
- Ensure no API keys or secrets are hardcoded
- Confirm Prisma queries are safe from injection
