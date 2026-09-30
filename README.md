# ScoutPay

**Verified work. Trusted proof. Stablecoin rewards.**

ScoutPay turns real-world verification into a trusted crypto-native work network. Sponsors lock rewards in escrow, contributors submit location-based proof, AI helps validate submissions, and approved workers receive instant stablecoin payments.

## Links

- **Live app:** https://scoutpay.lovable.app
- **Demo video:** https://youtu.be/l9NlpKf7nuY

## What it is

A mobile-first web app where organizations post real-world verification tasks (check an EV charger, map Wi-Fi speed, confirm shelter capacity) and contributors earn USDC after submitting proof: GPS location, photo, timestamp, an optional sensor reading, and a short note.

## Core flows

1. **Dashboard** — wallet status, earned USDC, pending review, reputation score.
2. **Tasks** — map-style panel plus task cards, filtered by DePIN, Payments, Infrastructure, Humanitarian, Connectivity.
3. **Task detail** — instructions, reward, sponsor, escrow status ("Reward locked in smart contract"), proof checklist.
4. **Submit proof** — photo upload, auto-detected GPS + timestamp, note, mock AI validation (location match, image relevance, duplicate check, risk score).
5. **Review** — approve or reject submissions; approval releases USDC to the worker wallet with a transaction and proof hash.
6. **Reputation** — trust score, approval rate, total earned, and badges (Reliable Verifier, Connectivity Mapper, Emergency Helper, Merchant Scout).
7. **Sponsor dashboard** — create campaigns, track budget vs. escrowed USDC, review submitted proofs.

## Demo mode

A toggle in the header seeds the guided flow: connect wallet → pick "Verify EV charger status" → start → submit proof → AI validates → approve → USDC released → reputation ticks up.

## Tech

- TanStack Start (React 19, Vite, Tailwind CSS v4)
- All state in the browser (React context + local storage) — no backend required
- Wallet connection, escrow, payouts, and hashes are realistic simulations, ready to swap for real Solana/EVM contracts

## Documents

- `ScoutPay_Project_Description.pdf` — full project description
- `ScoutPay_Pitch_Deck.pptx` — pitch slides
- `ScoutPay_Product_Walkthrough_v4.mp4` — narrated product walkthrough
