# Blackjack Academy

A responsive browser-based blackjack learning simulator with a casino-inspired practice table. Virtual chips only; progress is stored locally in the browser.

## Run locally
Open index.html in a modern browser. No build tools, package manager, API key, server or database required.

## Publish with GitHub Pages
1. Open Settings → Pages in this repository.
2. Under Build and deployment, choose Deploy from a branch.
3. Select main and /(root), then Save.
4. Wait for the Pages URL shown in that section.

## Included in this prototype
- Responsive blackjack practice table with hit, stand and double
- Dealer play, natural blackjack payout and customisable table settings
- Virtual bankroll, session record and local browser persistence
- Learning centre and compact basic-strategy reference
- Odds lab estimating next-card bust probability from the remaining shoe
- Hi-Lo card-counting practice with running and true count
- No real-money wagering, deposits or prizes

## Known limitations
Pair splitting is not implemented yet (the interface marks it as coming soon). The strategy coach and chart are simplified learning aids, not a complete rules-specific basic-strategy solver. Double-after-split and shoe penetration are saved as settings but not fully modelled. Further work should add split hands, insurance, a complete strategy engine, cut-card penetration and validated statistical simulations.

## Responsible play
This is an educational simulation, not financial advice or a way to guarantee wins. Basic strategy cannot remove the house edge under ordinary casino rules. Never gamble money you cannot afford to lose.
