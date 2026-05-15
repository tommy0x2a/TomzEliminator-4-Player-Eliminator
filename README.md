# TomzEliminator — 4 Player Multiplayer Edition

A browser-based recreation of the 1981 arcade game **Eliminator** by Gremlin, now with full real-time **4-player online multiplayer** using PeerJS.

## 🎮 Controls (Same for All Players)

| Key | Action      |
|-----|-------------|
| **D** | Turn Left   |
| **F** | Turn Right  |
| **J** | Thrust      |
| **K** | Fire        |

Every player uses the exact same keys. You only control your own ship.

## 👥 Player Setup

| Player   | Color    | Starting Corner | Role      |
|----------|----------|------------------|-----------|
| 1        | Cyan     | Top-Left         | **Host**  |
| 2        | Magenta  | Top-Right        | Guest     |
| 3        | Yellow   | Bottom-Left      | Guest     |
| 4        | Green    | Bottom-Right     | Guest     |

Guests join in order: **Magenta → Yellow → Green**.

## 🚀 How to Play Multiplayer

### As the Host
1. Click **CREATE ROOM (4P MULTIPLAYER)**
2. Copy and share the **Room Code** with your friends
3. Wait for all players to join
4. Click **START GAME** when everyone is ready

> **Important**: There is **no auto-start**. You control when the game begins so late joiners aren't instantly killed by the Eliminator.

### As a Guest
1. Click **JOIN ROOM (4P MULTIPLAYER)**
2. Paste the Room Code from the host
3. Your color and ship will be assigned automatically
4. Wait for the host to start the game

## 🕹️ Gameplay

- Destroy the central **Eliminator Base** by firing into its tunnel
- Shoot **Fighters** and the **Eliminator Enemy** for points and droids
- Ram/push enemies into the base for big bonuses
- You start with **12 lives**
- When you run out of lives, you become a **spectator** and can continue watching
- The last surviving player can press **R** to restart the match with the same players

## ✨ Key Features

- True 4-player real-time multiplayer (PeerJS)
- Host runs the authoritative simulation
- Guests get smooth extrapolated movement
- Visual explosions when player ships are destroyed
- Spectator mode for eliminated players
- Manual start button (prevents unfair early deaths)
- Live score + lives HUD positioned outside the play area
- Dynamic glowing border showing the current leader
- Full retro vector/neon 1981 aesthetic

## 📁 Single File Game

Everything is contained in one `index.html` file:
- HTML + CSS
- Full JavaScript game engine
- PeerJS multiplayer
- Synthesized audio (no external files)

Just open `index.html` in any modern desktop browser.

## 🛠️ Technical Details

- Built with vanilla HTML5 Canvas 2D
- PeerJS for peer-to-peer WebRTC connections
- Host-authoritative model with client-side prediction
- Works great on desktop keyboards

## 📜 Credits

Original arcade game: **Eliminator** © Gremlin Industries, 1981  
4-player multiplayer recreation & enhancements: Tommy (tommy0x2a)

Have fun blasting each other (and the base)! 🚀
