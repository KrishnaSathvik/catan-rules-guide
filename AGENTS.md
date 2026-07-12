# Catan Rules Guide

A static website (plain HTML/CSS/JS) served from `public/`. There is no build step, no
automated tests, and no linter configured — the "app" is just the static files in `public/`
(`index.html`, `seafarers.html`, `randomizer.html`, images, etc.). Deployment is via Vercel
(`vercel.json`, `outputDirectory: public`, `buildCommand: null`).

## Cursor Cloud specific instructions

- Run the dev server with `npm run dev` (defined in `package.json` as `npx serve public`); it
  serves on `http://localhost:3000`.
- Gotcha: the very first `npx serve` invocation on a cold npm cache prompts interactively
  (`Ok to proceed? (y)`), which hangs non-interactive shells. The update script pre-warms the
  `serve` package so `npm run dev` starts without prompting. If you ever hit the prompt anyway,
  run `npx --yes serve public` instead.
- `serve` uses clean URLs, so requesting `/index.html` (etc.) returns a `301` redirect to the
  extensionless path (`/`). Fetch `http://localhost:3000/` and `http://localhost:3000/randomizer`
  rather than the `.html` paths when checking status codes.
- Zero-dependency alternative (no network / npm needed): `python3 -m http.server 3001 --directory public`
  (this is what `.claude/launch.json` uses, on port 3001).
- There is nothing to build/lint/test: `npm run build` just echoes a message. Verify changes by
  loading the pages in a browser and exercising the interactive tools (Dice Roller tab on the base
  guide, and the Map Randomizer at `/randomizer`).
