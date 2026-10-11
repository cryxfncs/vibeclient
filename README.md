# Vibe Client

A Fabric utility client for **Minecraft 1.21.11**. Custom menus, a draggable HUD, an RGB theme system, and built-in Spotify integration — everything configurable in-game in **English, Deutsch, or العربية**.

## ✨ Features

- **Animated main menu** — procedural sunset panorama with parallax, live clock, and themed Singleplayer / Multiplayer / Options / Quit buttons
- **ClickGUI (`Right Shift`)** — animated module list with toggles, Spotify mini-player with playback controls, and quick access to Theme, Language, 3D menu, and HUD editor
- **3D Ground Menu** — the module list projected onto the ground 3 blocks ahead of you: **left-click toggles**, **right-click opens the module's settings**
- **Draggable HUD editor (`H`)** — move Watermark, TopBar, Stats, Keybinds, Armor, and Spotify pills freely; TopBar snaps back to center on right-click
- **RGB theme system** — Chroma, Static, Fade, and Sweep modes with adjustable colors and animation speed, applied to every UI element
- **Per-module settings** — right-click any module for sliders and toggles, saved automatically to `config/vibeclient-modules.json`
- **Toasts, custom nametags with HP bars, and theme-colored hitboxes** (a visual alternative to F3+B)

## 🎵 Spotify integration

- **Web API mode**: `/spotify setup <id> <secret>` once (free app at `developer.spotify.com/dashboard`), then `/spotify login` — browser OAuth with local callback, track display, play / pause / next / previous from chat or ClickGUI
- **Synced + plain lyrics** via lrclib, shown as an in-game overlay
- **Window-title fallback**: shows the current track from the Spotify window title when the Web API isn't linked
- Required Redirect URI in the Spotify dashboard (exact match): `http://127.0.0.1:8917/callback`

## 📦 Modules

CustomHUD, Nametags, Hitboxes, Spotify, Zoom, ArmorHUD, Sprint, Fullbright, Fly, Aimbot, KillAura.

## ⌨️ Keybinds & Commands

- `Right Shift` — ClickGUI · `H` — HUD editor (both rebindable under Controls)
- `/spotify login | setup | logout | status | lyrics | play | pause | next | prev`

## 🔧 Requirements

Fabric Loader **0.19.5**, Fabric API, Fabric Language Kotlin. Sodium / Sodium Extra are supported but optional.

## 📁 Configuration files

All settings persist in `config/`: `vibeclient-modules.json`, `vibeclient-hud.json`, `vibeclient-theme.json`, `vibeclient-lang.json`, `vibe-client-spotify.json`.
