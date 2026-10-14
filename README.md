# $KOTH — King of the Hill

The hill is back. Every pump.fun coin is ranked live. Take the crown.

## Files

- `index.html` — the whole site (live leaderboard, wallet connect, styles, logo).
- `vercel.json` — lets the site read pump.fun's coin list through your own domain (`/pf/...`).

## Deploy on Vercel

1. Put both files at the root of a GitHub repo.
2. In Vercel: Add New → Project → Import the repo.
3. Framework preset: Other. Leave build command and output directory empty.
4. Deploy.

## Check it works

- https://www.koth.fun/pf/coins?offset=0&limit=5&sort=market_cap&order=DESC&includeNsfw=false shows pump.fun coins.
- On the homepage the dot next to [connect wallet] turns green and says "live".

## Settings

Edit the `CONFIG` block at the top of the `<script>` in `index.html`:
`KOTH_MINT` (your token address), `RPC_URL` (a dedicated Solana RPC such as Helius), `LINKS.telegram`.
