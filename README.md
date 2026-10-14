# TNZ HEROES — Telegram Mini App (v2.0)

TNZ HEROES — single-page browser game / Telegram Mini App prototype in Russian. It is built with plain HTML, CSS and JavaScript; no build step is required.

## Run locally

1. Extract the ZIP.
2. Open `index.html` in a modern browser.
3. Game progress is saved locally in the browser (`localStorage`).

For a Telegram Mini App, host `index.html` at a public HTTPS URL, then configure that URL for a Telegram bot via `@BotFather` (Web App / Menu Button). The Telegram Web Apps SDK is included.

## Features

- Animated TNZ HEROES loading screen and responsive mobile UI.
- Six selectable characters with distinct base stats and special abilities.
- Hero levels, XP, power/defense/health upgrades and a strength rating.
- Daily login rewards with a login streak.
- Daily quests for battles, upgrades, training and login rewards.
- Turn-based PvE battles against bots, with easy / normal / boss difficulty.
- Attacks, character skills, defense, energy meter, healing potions, combat log and battle history.
- Gear shop with weapons, armor, relics, healing potions, XP elixirs and loot chests.
- Inventory and equipment slots; equipped gear affects combat stats.
- Eight claimable achievements.
- Player profile, editable display name, sound toggle and animation toggle.
- JSON save export/import and progress reset.
- Optional Telegram haptic feedback and display-name suggestion.

## Important limitations

This is a playable frontend prototype. Coins, quests, opponents and player data are simulated locally and can be modified by the player. The leaderboard / real multiplayer / anti-cheat / real reward delivery to a Minecraft server are not implemented. For a public release, add a backend and database, validate Telegram `initData` on the server, and have the backend authoritatively handle balances, daily claims, battle rewards and quest completion. Never trust `initDataUnsafe` or client-side currency as proof of identity/reward entitlement.
