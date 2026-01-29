---
name: query-optimizer
description: Optimize SQL and Prisma queries with AI. Use when queries are slow.
---

# Query Optimizer

Your queries are slow but EXPLAIN output is confusing. This tool analyzes your queries and tells you exactly how to make them faster.

**One command. Zero config. Just works.**

## Quick Start

```bash
npx ai-query-optimize ./src/queries/
```

## What It Does

- Analyzes SQL and Prisma queries
- Identifies N+1 queries and missing indexes
- Suggests query rewrites for better performance
- Explains why changes improve speed

## Usage Examples

```bash
# Analyze query files
npx ai-query-optimize ./src/queries/

# Analyze Prisma client usage
npx ai-query-optimize ./prisma/
```

## Best Practices

- **Use EXPLAIN** - understand what the database is doing
- **Batch queries** - avoid N+1 with includes/joins
- **Index where clauses** - most common optimization
- **Limit results** - don't fetch more than needed

## When to Use This

- Queries are getting slow as data grows
- Database load is too high
- Need to optimize before launch
- Learning query optimization

## Part of the LXGIC Dev Toolkit

This is one of 110+ free developer tools built by LXGIC Studios. No paywalls, no sign-ups, no API keys on free tiers. Just tools that work.

**Find more:**
- GitHub: https://github.com/LXGIC-Studios
- Twitter: https://x.com/lxgicstudios
- Substack: https://lxgicstudios.substack.com
- Website: https://lxgicstudios.com

## Requirements

No install needed. Just run with npx. Node.js 18+ recommended. Needs OPENAI_API_KEY environment variable.

```bash
npx ai-query-optimize --help
```

## How It Works

Reads your query files, identifies patterns that cause performance issues like N+1 queries or missing indexes. The AI suggests specific optimizations with before/after examples.

## License

MIT. Free forever. Use it however you want.
