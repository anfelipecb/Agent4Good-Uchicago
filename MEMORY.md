# Agents4Good — project memory

Concise facts for anyone (or any agent) updating this repo.

## What this is

UChicago student-led group site: landing page, per-session invite cards, links to community tools and session artifacts. **Production:** [agents4good-uchicago.vercel.app](https://agents4good-uchicago.vercel.app/)

## Deploy

- **Host:** Vercel, static HTML/CSS (no build).
- **Trigger:** Push to `main` on the connected Git repo should redeploy production. If production looks stale while GitHub `main` is correct, open the Vercel project → **Deployments** and confirm builds are running for new commits; reconnect the Git integration under **Settings → Git** if needed.
- **CLI fallback:** `vercel deploy --prod` from this directory (requires Vercel CLI login). Large files under `sessions/*/docs/` are excluded via [`.vercelignore`](.vercelignore) so uploads stay small.

## Repo layout

| Path | Role |
|------|------|
| `index.html` | Main site: hero, sessions, resources |
| `styles.css` | Shared styles for main site |
| `sessions/NN/index.html` | Invite / detail card for session NN (inline CSS) |
| `sessions/NN/og-image.png`, `og-card.html` | Social preview assets where used |
| `sessions/NN/docs/` | Optional local exports (recordings, etc.); large binaries are gitignored |

## External URLs (update here when links change)

| Label | URL |
|-------|-----|
| WhatsApp community | `https://chat.whatsapp.com/GzSpVxexoOY7VSEWYeN89o` |
| Session feedback survey (Google Form) | `https://docs.google.com/forms/d/e/1FAIpQLSfkgSbDQpfHfa1FP5H-t80bUhdJW2nWBRiSUUkGJ8nTYz9L9Q/viewform?usp=dialog` |
| Meeting time poll (crab.fit) | `https://crab.fit/ai-agent-group-meeting-time-300995` |
| Session 01 notes (Notion) | `https://www.notion.so/analyticpr/3301c4d77bd7801aab6dc539595d9fb1?source=copy_link` |
| Session 02 notes (Notion) | `https://www.notion.so/analyticpr/3371c4d77bd780c6a544dc501adbde97?source=copy_link` |
| Session 02 recording (Box) | `https://uchicago.box.com/s/g841v0diyoy6suo3u3nt7nhdlpa3titu` |
| Session 02 Zoom (historical) | `https://uchicago.zoom.us/j/98515018610?pwd=RD3BpszK168KEPIO8bxgmd8YSKmBgg.1` |

## Conventions

- Prefer `target="_blank"` and `rel="noopener noreferrer"` on external links.
- After sessions ship, add Notion + recording links on both the main `index.html` session card and `sessions/NN/index.html`.
- When adding new session links, update this file and the **Resources** section on the site if needed.
