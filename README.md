# Blackjack Academy

A responsive browser-based blackjack learning simulator with a premium casino-inspired practice table. Virtual chips only; no cash value, deposits or prizes.

## Run locally
Open index.html in a modern browser. The standalone game requires no build tools. Global accounts and leaderboard connect to Supabase.

## Publish with GitHub Pages
1. Open Settings → Pages in this repository.
2. Under Build and deployment, choose Deploy from a branch.
3. Select main and /(root), then Save.
4. Wait for the Pages URL shown in that section.

## Included
- Premium emerald-and-gold casino visual refresh with animated cards
- Blackjack practice table with hit, stand and double
- Dealer play, natural blackjack payout and customisable table settings
- Learning centre, simplified strategy reference, odds lab and Hi-Lo count trainer
- Player accounts and global top-10 leaderboard
- Cross-device bankroll and hand-count sync for signed-in players
- £200 daily recovery allowance, available the day after a player's bankroll reaches zero
- Local practice remains available without an account

## Supabase setup
The production project is configured in Supabase. The browser uses the project URL and publishable key in `index.html`; publishable keys are designed for client use and database access is restricted with Row Level Security and authenticated RPCs.

In Supabase Dashboard → Authentication → URL Configuration, set the Site URL to:
`https://cammyc1.github.io/Blackjack-academy/`
Add the same URL to the Redirect URLs allow-list so email confirmation returns players to the site.

New players create an account with an email, password and unique 3–18 character username. If email confirmation is enabled, they must confirm their email before signing in. Then they can join the leaderboard.

## Leaderboard integrity
The leaderboard is a friendly virtual-chip competition. Game decisions and bankroll are currently calculated in the browser and submitted by the signed-in player, so this first version is **not tamper-proof** and must not be used for cash prizes or valuable rewards. A future competitive release would need authoritative server-side hand dealing and settlement.

## Known limitations
Pair splitting is not implemented yet (the interface marks it as coming soon). The strategy coach and chart are simplified learning aids, not a complete rules-specific basic-strategy solver. Double-after-split and shoe penetration are saved as settings but not fully modelled. Further work should add split hands, insurance, a complete strategy engine, cut-card penetration and validated statistical simulations.

## Responsible play
This is an educational simulation, not financial advice or a way to guarantee wins. Basic strategy cannot remove the house edge under ordinary casino rules. Never gamble money you cannot afford to lose.
