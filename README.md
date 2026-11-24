# PixelPlay Arcade

A responsive, static browser arcade with five original mini-games. No build step or backend is required.

## Included

- Reaction Rush — five-round reaction-time challenge
- Memory Match — eight-pair memory game
- Neon Snake — keyboard and on-screen directional controls
- Target Tap — timed target clicking challenge
- 2048 Dash — keyboard-controlled number merge puzzle
- Search and category filters
- Nickname, personal scores and round count stored in browser local storage
- About, privacy and terms pages, plus sitemap and robots.txt

## Run locally

Open `index.html` in a modern browser, or serve this folder with any static file server. No dependencies or build command are required. Google Fonts are optional; system fallbacks are included.

## Deploy to Netlify

Connect this GitHub repository to Netlify and set:

- Production branch: `main`
- Build command: leave blank
- Publish directory: `.`

Every push to `main` can then publish automatically.

## Important limitations before public launch

- Scores and nicknames are stored locally on one browser/device. This is not a shared global leaderboard or account system.
- Advertising is not included or enabled. Do not add ads beside game controls or inside active gameplay.
- Replace the placeholder contact address in the policy pages with a monitored address before launch.
- Update the canonical URL and sitemap if the final Netlify subdomain differs.
- Review legal and privacy wording for the operator's jurisdiction and any analytics/ad providers before enabling them.

## License

No third-party game assets are bundled. Contact the repository owner for reuse permission.
