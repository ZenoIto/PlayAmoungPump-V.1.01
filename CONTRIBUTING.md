# Play AmoungPump

**One minute. Eight crew members. Two hidden Ruggers. Trust no one.**

---

## Overview

**AmoungPump** is a browser-based social deduction game set aboard Genesis Station. In every round, six Traders try to complete the station’s network tasks while two hidden Ruggers sabotage the mission, eliminate crew members and avoid being voted out.

You play as **Mission Control**. Follow the crew, complete assignments, investigate suspicious activity and cast your vote when a meeting begins.

This release is a **local demo**. Characters use programmed behavior, and every visitor runs an independent game in their own browser.

---

## Key Features

**One-Minute Rounds** – Rounds have a 60-second deadline. A decisive victory can end a round earlier; the next begins after a 10-second intermission.

**Social Deduction** – Observe eight autonomous characters, review events and vote for a suspect during meetings.

**Expanded Station** – Explore 10 connected rooms using zoom, drag controls and character-following camera movement.

**Playable Assignments** – Solve three interactive challenges each round to contribute to the Traders’ task goal.

**Mission Control** – Spend limited energy to scan activity, activate Overdrive or restore the lights after sabotage.

**Detective Progression** – Predict a Rugger to earn XP and build a streak saved in your browser.

**Demo Gacha** – Open one capsule after each round to receive simulated $AMOUNG. Official token rewards are planned for a future update.

**Instant Play** – No account, wallet, API key or installation is needed to play in a browser.

---

## Technology Stack

- **Languages:** HTML, CSS and JavaScript
- **Graphics:** HTML Canvas
- **Game engine:** Local rules for movement, roles, tasks, sabotage, meetings and voting
- **Persistence:** Browser storage for usernames and local progression
- **Hosting:** Static hosting, including Netlify
- **External APIs:** None required for the current demo

---

## Installation

Clone the repository and serve the `dist` folder with a static file server:

```bash
git clone https://github.com/ZenoIto/PlayAmoungPump-V.1.01.git
cd PlayAmoungPump-V.1.01
python3 -m http.server 8000 --directory dist
```

Open **http://localhost:8000** in your browser.

For a manual Netlify deployment, upload the complete **`dist` folder**.

---

## Usage

### 1. Enter Genesis Station

Watch or skip the introduction, choose a username and select **Enter Genesis**. Your username is remembered in the same browser.

### 2. Explore the Map

Follow the crew as they move between rooms. Zoom in, drag the map to inspect an area or select a character to follow them.

### 3. Complete Assignments

Use the task panel to:

- Reconnect nodes in the correct sequence.
- Tune the reactor to its target level.
- Match the cargo seal.

Each completed assignment contributes one network task. Every round offers fresh challenges.

### 4. Investigate and Vote

Use Mission Control tools to gather clues and respond to sabotage. When a meeting begins, review the evidence and cast your vote. You can also predict a Rugger to earn detective XP.

### 5. Open a Demo Capsule

After the round, open your free capsule during the intermission. Demo $AMOUNG balances are simulated, have no monetary value and cannot be withdrawn.

---

## Example Round

```text
Username: PumpPilot
Location: Genesis Station
Crew: 6 Traders · 2 Ruggers
Trader objective: Complete 22 network tasks or eject both Ruggers
Round deadline: 60 seconds

Your options:
→ Follow the crew
→ Complete assignments
→ Scan activity
→ Respond to sabotage
→ Vote during meetings
→ Open a demo capsule after the round
```

---

## Error Handling

The entry form validates usernames before starting the game. If browser storage is unavailable, you can still play the current session, although your progress may not be saved.

When the browser tab becomes inactive, the local simulation pauses instead of skipping unseen gameplay.

---

## Planned Updates

- Official gacha system
- Future $AMOUNG integrations
- Staking features

**These features are not live in the current demo.** There are no wallet connections, blockchain transactions or real-money rewards.

---

## Contributing

Feedback and contributions are welcome. Open an issue to report a bug or propose a feature, or submit a pull request with your changes.

---

## License

No license has been specified yet. A `LICENSE` file should be added before granting permission to reuse or distribute the code.
