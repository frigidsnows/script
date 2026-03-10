# gobblegum

![Version](https://img.shields.io/badge/version-2.x-purple)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Platform](https://img.shields.io/badge/platform-Roblox-red)
![License](https://img.shields.io/badge/license-MIT-blue)
![Maintained](https://img.shields.io/badge/maintained-yes-success)

A web-connected Roblox client script focused on syncing cosmetic items, visual effects, and social features between users in real time.

`gobblegum` links a Roblox script with a small web backend so players using the script can automatically share avatar items, visual effects, and chat across servers.

---

# Features

## Loadout Sync

Players using the script can share avatar cosmetics across servers.
When someone uploads their loadout, other users running the script will automatically see those items applied locally.

Supported content includes:

* Accessories
* Clothing
* Body meshes
* MeshPart avatars
* Faces and head meshes
* Animations and emotes

Everything is applied locally, meaning the actual Roblox avatar is never permanently modified.

---

## Avatar Rendering System

The script creates a **visual layer** that renders synced items on the character without modifying the real avatar.

This system handles:

* accessory attachments
* head mesh replacement
* clothing overrides
* body mesh swapping
* animation injection

Because this layer is separate from the original character, items can be added or removed dynamically.

---

## Player Tags

Players running the script automatically receive a tag above their character.

Tag system includes:

* custom icon support
* animated text
* user roles (owner / admin / user)
* customizable colors
* optional rainbow effects

Tags are also interactive — clicking a player tag can teleport you behind them.

---

## Visual Effects

The script includes several cosmetic effects designed to make synced players easier to recognize.

Available effects:

* highlight aura around users
* particle emitters
* recolored fire effects
* animated teleport visuals
* optional teleport sounds

These effects trigger dynamically when events occur in-game.

---

## Teleport Detection

When a player moves a large distance instantly, the script detects it and triggers a visual effect.

Teleport effects include:

* expanding energy ring
* light pillar animation
* camera FOV pulse
* optional teleport sound

This system makes fast movements more noticeable and visually styled.

---

## Global Shoutbox

A built-in global chat system allows users running the script to communicate across servers.

Features:

* draggable chat window
* resizable interface
* message history
* private messaging
* admin commands

Supported commands:

```
/pm [user] [message]
/kick [user]
/ban [user]
```

Messages are synced through the backend API and refreshed periodically.

---

## Avatar Preview

The script includes a preview renderer that displays a 3D model of synced cosmetics.

Preview system features:

* viewport rendered character
* optional model rotation
* real-time updates
* UI toggle support

---

# Screenshots

*(Replace with your own screenshots if uploading to GitHub)*

## Player Tags

<img width="796" height="96" alt="image" src="https://github.com/user-attachments/assets/89422161-d9db-4e4a-80b9-7a899874c27b" />


---

## Teleport Effects

<img width="784" height="268" alt="image" src="https://github.com/user-attachments/assets/6c048137-dd37-4759-b6cf-abb7148a37fc" />


---

## Global Shoutbox

<img width="353" height="338" alt="image" src="https://github.com/user-attachments/assets/0bccce26-e3dc-417f-8681-fe96d19bfd65" />


---

## Avatar Preview

<img width="275" height="333" alt="image" src="https://github.com/user-attachments/assets/c9d0ae77-6b9b-4eca-94de-8f9a368d0afe" />


---

# Feature GIFs

*(Optional animated previews)*

### Teleport Effect

![ow-overlay_nHJYr5Vqix](https://github.com/user-attachments/assets/794ecc81-75b0-4cae-952a-aeb6cc37c6e5)

### Tag Animation

![ow-overlay_sHgU9ESCPS](https://github.com/user-attachments/assets/01725b13-d048-4c64-951c-f16d668c5ca4)


### Emote Wheel Injection

<img width="680" height="504" alt="image" src="https://github.com/user-attachments/assets/a6de0827-3e22-48b1-8eea-44df6c6a2e7e" />

## Full menu

![ow-overlay_XgtMD3UcWB](https://github.com/user-attachments/assets/d63c04fb-1beb-4484-829c-022c7f40703e)

---

# Backend API

The script communicates with a small web backend to synchronize data between users.

Endpoints used by the client include:

```
/api/get-all
/api/get-loadout/:userid
/api/save
/api/chat
```

These endpoints provide avatar loadouts and chat messages that are synced across players.

---

# Requirements

Some features rely on executor capabilities such as:

* HTTP requests
* file access
* custom asset loading

Without these, certain features (like global chat or sound downloads) may not function.

---

# Disclaimer

This project is experimental and intended for learning or private environments.

Use responsibly and ensure that your environment allows client-side modifications.

---

# License

MIT License

Copyright (c) gobblegum

Permission is granted to use, modify, and distribute this project under the terms of the MIT license.
