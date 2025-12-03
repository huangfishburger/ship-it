# 🛒 Ship It

The application is built with [Bun](https://bun.sh/), [React](https://reactjs.org/), [TypeScript](https://www.typescriptlang.org/), [Next.js](https://nextjs.org/) and [Shadcn UI](https://ui.shadcn.com/).

## 💡 Introduction
This project is a database-backed inventory system to manage and visualize e-commerce sales and stock data. It aimed to streamline data updates, monitor key metrics in real time, and support data-driven ordering decisions.

**(Note on Authorship): This repository is a derivative copy of the original team project. The code represents the combined efforts of the development team listed below. My primary contributions focused on UI, dashboard and database design**

## 🔧 Setup

```bash
cp .env.example .env
```

Edit the `.env` file with your own values.

## 💻 Development

```bash
# Install dependencies
bun install

# Run the application
bun run dev

# Lint
bun run lint
```

When the application is running, you can access the application at [http://localhost:3000](http://localhost:3000).

## ⚡️ Supabase

## Init

```bash
# Login 
bun run supabase login

# Link DB
bun run supabase link --project-ref <project-id>
```

## Migrations

```bash
# Create migration
bun run supabase migration new <name>

# List migrations
bun run supabase migration list

# Push migration
bun run supabase db push

# Generate types
bun run supabase gen types typescript --project-id <project-id> --schema public > database.types.ts

# Revert migration
bun run supabase migration repair --status reverted <migration-id>
```
