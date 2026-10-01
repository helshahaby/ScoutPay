Build a polished mobile-first (android .apk) web app called ScoutPay.

ScoutPay is a DePIN + crypto payments app where organizations post real-world verification tasks and users earn stablecoin rewards after submitting proof such as GPS location, photo, timestamp, sensor result, and a short note.

The app should feel like a serious hackathon MVP/startup product, not a landing page. Build the usable product first.

Core screens:
1. Dashboard
- Show user wallet status, total earned, pending rewards, completed tasks, reputation score.
- Add a “Connect Wallet” button.
- Show quick stats: Available Tasks, Pending Review, Earned USDC, Reputation.

2. Task Map / Task List
- Show nearby verification tasks in cards and on a simple map-style panel.
- Each task should include title, category, location, reward in USDC, urgency, required proof, and deadline.
- Example tasks:
  - Verify EV charger status
  - Check public Wi-Fi speed
  - Confirm shelter capacity
  - Report damaged road sign
  - Verify crypto payment accepted by merchant
- Add filters for DePIN, Payments, Infrastructure, Humanitarian, Connectivity.

3. Task Detail
- Show full instructions, reward amount, proof requirements, sponsor name, and estimated time.
- Add button “Start Task”.
- Show escrow status: “Reward locked in smart contract”.
- Show required proof checklist:
  - GPS location
  - Photo
  - Timestamp
  - Short note
  - Optional sensor/speed result

4. Submit Proof
- Let user upload/take a photo.
- Show detected GPS coordinates, timestamp, and note field.
- Add mock AI validation result:
  - Location match
  - Image relevance
  - Duplicate check
  - Risk score
- Button: “Submit for Review”.

5. Review / Validation
- Show pending submissions.
- Include AI proof score, photo thumbnail, submitted note, task location, and fraud risk.
- Reviewer can Approve or Reject.
- If approved, show “USDC released to worker wallet”.

6. Reputation
- Show worker profile with completed tasks, approval rate, total earned, badges, and trust score.
- Badges:
  - Reliable Verifier
  - Connectivity Mapper
  - Emergency Helper
  - Merchant Scout

7. Sponsor Dashboard
- Let an organization create a task campaign.
- Inputs: task title, category, location, reward, number of verifications needed, deadline, proof requirements.
- Show campaign budget and total USDC escrowed.
- Show submitted proofs and status.

Crypto/Web3 behavior:
- Use mock wallet connection if real wallet integration is not available.
- Show wallet address after connection.
- Simulate USDC escrow and payout.
- Show transaction hash after approval.
- Show on-chain proof hash for each approved submission.
- Make clear this is a working MVP simulation that can later connect to Solana/EVM smart contracts.

Design:
- Clean, modern, trustworthy.
- Mobile-first but responsive on desktop.
- Use a professional color palette, not too dark and not purple-heavy.
- Use cards only for task items and submissions.
- Use tabs or sidebar navigation: Dashboard, Tasks, Submit Proof, Review, Sponsor, Reputation.
- Use icons for wallet, map, camera, shield, payment, reputation.
- Add subtle animations when tasks are approved or payment is released.
- Keep text concise and practical.

Important UX:
- The first screen should be the app dashboard, not a marketing hero.
- Include realistic sample data.
- Include empty/loading/error states.
- Prevent text overflow on mobile.
- Add a demo mode toggle so judges can understand the flow quickly.

Demo flow:
1. Connect wallet.
2. Choose “Verify EV charger status”.
3. Start task.
4. Submit photo/GPS/note proof.
5. AI validates proof.
6. Reviewer approves.
7. USDC reward is released.
8. Reputation score increases.

Add a short “Why ScoutPay?” section inside the app, not as the main page:
“ScoutPay turns real-world verification into a trusted crypto-native work network. Sponsors lock rewards in escrow, contributors submit location-based proof, AI helps validate submissions, and approved workers receive instant stablecoin payments.”

Make it production-looking enough for a Colosseum crypto hackathon submission.
