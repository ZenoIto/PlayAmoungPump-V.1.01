# Play AmoungPump

**A one-minute social deduction game. Complete the mission. Find the Ruggers. Trust no one.**

---

## Overview

**AmoungPump** is a browser-based social deduction game set aboard Genesis Station. Each round brings together six Traders and two hidden Ruggers. Traders work to complete the station’s network tasks, while Ruggers sabotage the crew, eliminate players and try to survive the vote.

You join as **Mission Control**. Choose a username, watch the crew move through the station, complete interactive assignments, investigate suspicious activity and cast your vote when a meeting begins.

The current release is a **local game demo**. Its characters follow programmed behavior; each visitor plays an independent simulation.

---

## Key Features

**One-Minute Rounds** – Each round has a 60-second deadline. A decisive win can end it earlier, followed by a 10-second intermission before the next round.

**Social Deduction** – Observe eight autonomous characters, follow events, investigate suspects and vote during meetings.

**Expanded Station** – Explore a 10-room map with zoom, camera controls and multiple routes.

**Interactive Tasks** – Complete three playable assignments per round to help the Traders reach their network goal.

**Mission Control Tools** – Scan activity, activate Overdrive and restore the lights using limited energy.

**Detective Progression** – Predict a Rugger, build a streak and earn XP saved in your browser.

**Demo Gacha** – Open one capsule after each completed round for simulated $AMOUNG rewards. Official token rewards are planned for a future update.

**Instant Browser Play** – No installation, wallet connection, account or API key is required to play.

---

## Technology Stack

- **Languages:** HTML, CSS and JavaScript
- **Rendering:** HTML Canvas for the station, characters and effects
- **Game logic:** Local simulation with navigation, tasks, roles, meetings and voting
- **Storage:** Browser storage for the username and local progression
- **Hosting:** Static hosting, including Netlify
- **External services:** None required for the current demo

---

## Installation

To run the project locally, download or clone the repository and serve the `dist` folder with any static file server:

```bash
git clone https://github.com/ZenoIto/PlayAmoungPump-V.1.01.git
cd PlayAmoungPump-V.1.01
python3 -m http.server 8000 --directory dist
```

Then open `http://localhost:8000` in your browser.

To deploy manually on Netlify, upload the complete **`dist` folder** through your site’s deployment area.

---

## Usage

### 1. Enter Genesis Station

Watch or skip the introduction, enter a username and select **Enter Genesis**. Your username appears in the game and is remembered in the same browser.

### 2. Explore the Map

Watch the crew travel between rooms. Use the zoom controls and drag the map to inspect different areas. Select a character to follow them.

### 3. Complete Assignments

Open the task panel and solve the three available challenges:

- Reconnect nodes in the correct sequence.
- Tune the reactor to its target power.
- Match the cargo seal.

Each completed assignment adds one network task to the Traders’ progress.

### 4. Investigate and Vote

Use Mission Control actions to gather clues or respond to sabotage. During meetings, review what happened and cast your vote. You can also lock in a suspect prediction to earn detective XP.

### 5. Open a Demo Capsule

After a round ends, open the free demo gacha capsule during the intermission. The displayed $AMOUNG balance is **simulated** and has no monetary value.

---

## Example Round

```text
Username: PumpPilot
Round: Genesis Station
Crew: 6 Traders · 2 Ruggers
Mission: Complete 22 network tasks or eject both Ruggers
Time limit: 60 seconds

Mission Control:
→ Follow the crew
→ Complete an assignment
→ Scan suspicious activity
→ Vote during a meeting
→ Review the result and open a demo capsule
```

---

## Error Handling

The game checks usernames before entry and rejects invalid input. If browser storage is unavailable, the current session can still run, but saved progress may not persist.

The simulation pauses when the browser tab is inactive so that returning to the page does not skip unseen gameplay.

---

## Planned Updates

- Official gacha implementation
- Future $AMOUNG integrations
- Staking features

These features are **not live** in the current demo. The game has no wallet connection, blockchain transactions or real-money rewards.

---

## Contributing

Contributions and feedback are welcome. You can open an issue to report a bug or suggest an improvement, or submit a pull request with a proposed change.

---

## License

A license has not been specified for this project yet. Add a `LICENSE` file before describing the repository as open source or granting reuse rights.

