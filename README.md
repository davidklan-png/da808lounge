# Da 808 Lounge

**Live:** https://da808lounge.pages.dev

Static single-page site for Da 808 Lounge, a Hawaiian lounge in Takadanobaba, Tokyo (Sun Patio Takadanobaba 1F, 3-1-5 Takadanobaba, Shinjuku-ku). No build step, framework, or dependencies — everything the page needs is served as-is from [`public/`](public/). To deploy on Cloudflare Pages, create a Git-connected Pages project for this repo with no build command and **`public`** as the build output directory (or run `npx wrangler pages deploy public --project-name da808lounge`); every push to `main` redeploys automatically.

The Instagram section shows the account's latest 5 posts dynamically via Behold ([behold.so](https://behold.so)) — set `FEED_URL` in the loader script at the bottom of `public/index.html` to the feed's JSON endpoint; while it's empty (or if the fetch fails) a static photo fallback is shown instead.

Hours, review quotes, and the "Around the web" stats are curated snapshots of the bar's public listings (Google Maps, [Tabelog](https://tabelog.com/tokyo/A1305/A130503/13278819/), [Facebook](https://www.facebook.com/Da808Lounge/)) as of August 2026 — review quotes are verbatim Tabelog text; re-verify before reuse.
