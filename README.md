# Agents4Good

A University of Chicago student initiative exploring **agentic AI workflows** together: lightning talks, hands-on tooling, and shared resources. The public site lives at **[agents4good-uchicago.vercel.app](https://agents4good-uchicago.vercel.app/)**.

This repository is a **static** site (HTML + CSS). There is no bundler or server-side code.

## Local preview

From the repository root:

```bash
npx --yes serve .
```

Or with Python:

```bash
python3 -m http.server 8080
```

Then open the URL the command prints (often `http://localhost:3000` or `http://localhost:8080`).

## Deploy (Vercel)

The project is deployed on **Vercel**. With the GitHub (or Git) integration pointed at `main`, **every push to `main` triggers a production deploy**. No separate build command is required.

## Maintainer notes

See [MEMORY.md](MEMORY.md) for canonical external URLs and layout conventions.
