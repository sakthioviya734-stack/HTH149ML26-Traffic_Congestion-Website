# Smart Traffic Command Center

AI-driven municipal traffic intelligence interface, built from the
"Smart City Command" design system (TanStack Start + React 19 + Tailwind CSS v4).

## Screens

| Route | Screen |
| --- | --- |
| `/` | Welcome portal |
| `/login` | Operator sign in |
| `/intelligence` | Traffic intelligence portal |
| `/dashboard` | Officer command dashboard |
| `/prediction` | Congestion prediction |
| `/priority` | Priority locations |
| `/actions` | Recommended actions |
| `/analytics` | Traffic analytics |

A floating navigator (bottom-right) links every screen; sidebar items and
primary buttons also route to their matching pages.

## Run locally

```bash
bun install      # or: npm install
bun run dev      # http://localhost:8080
bun run build    # production build
```

## Structure

- `src/routes/` — one file per screen (file-based routing)
- `src/components/PageShell.tsx` — shared page wrapper + link routing
- `src/components/RouteSwitcher.tsx` — floating screen navigator
- `src/styles.css` — design tokens (colors, type scale, spacing, radii)
