# Questboard

The Active Quest Board card, at https://questboard.quest-engine.workers.dev
(Cloudflare, behind Roy's Cloudflare Access login), from `index.html`.

Its data comes from the Quest Engine (Cloudflare Worker,
`rdecaste/quest-engine`) at `GET /questboard`, rebuilt by the 03:00 journal
chain from the quests in its D1 database. How it works:
`docs/quest-engine.md` in rdecaste/quest-engine.

A push to `main` deploys it to Cloudflare (Workers Builds); by hand: `npx wrangler deploy`. Only the pages are published (`.assetsignore`). The old `rdecaste.github.io` address forwards here until GitHub Pages is switched off.
