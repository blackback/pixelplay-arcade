# PixelPlay Arcade

A responsive browser arcade with five mini-games and a Supabase-backed global leaderboard. The static frontend has no build step; the score submission service runs on Supabase Edge Functions.

## Included

- Reaction Rush — five-round reaction-time challenge
- Memory Match — eight-pair memory game
- Neon Snake — keyboard and on-screen directional controls
- Target Tap — timed target clicking challenge
- 2048 Dash — keyboard and touch number merge puzzle
- Search and category filters
- Guest nicknames, local personal stats and public global leaderboards
- Guest score submission through a server-side function with score bounds and IP-hash rate limits
- About, privacy and terms pages, plus sitemap and robots.txt

## Run locally

Open `index.html` in a modern browser, or serve this folder with any static file server. The global leaderboard and score submissions require the configured Supabase project.

## Deploy to Netlify

Connect this GitHub repository to Netlify and set:

- Production branch: `main`
- Build command: leave blank
- Publish directory: `.`

Every push to `main` can then publish automatically.

## Backend

The Supabase project provides the public best-score view and the `submit-score` Edge Function. The function uses a server-side secret key; never put that key in frontend code. The database function validates game slugs, score ranges and nickname format, and applies a per-IP-hash cooldown and daily submission limit.

## Important limitations

- No player account, email or password is required. Nicknames are not verified identities and can be impersonated.
- The games run in the browser, so server-side score bounds and rate limits reduce abuse but do not make client-generated scores fully cheat-proof.
- Advertising is not included or enabled. Do not place ads beside game controls or inside active gameplay.
- Replace the placeholder contact address in the policy pages with a monitored address before public launch.
- Review legal and privacy wording for the operator's jurisdiction and any analytics/ad providers before enabling them.

## License

No third-party game assets are bundled. Contact the repository owner for reuse permission.
