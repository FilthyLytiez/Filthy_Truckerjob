# 🚛 Filthy Truckerjob v1 — Qbox & QBCore Compatible

Welcome to **Filthy Truckerjob**, a two-in-one trucking mission system with *kasi flavor* and full sync. Whether you're running legal cargo for Mkize or pulling off dangerous illegal deliveries, this script is fully optimized for Qbox or QBCore.  
It supports dispatch, fuel scripts, target systems, and has built-in cooldowns and NPC action. 💰🔫🇿🇦

---

## 📦 Features

### 🚚 Legal Trucking Jobs
- Multiple delivery routes per job
- Safe delivery points, no enemies
- Trailer and cargo system
- Legit business operation for clean RP servers

### 🦹‍♂️ Illegal Trucking Heists
- One high-risk delivery
- Armed NPCs spawn and attack!
- Sends police dispatch alerts
- Trailer destruction = mission failed
- Big payout if successful

### 👨‍🔧 Fully Synced System
- Trailer must be attached or you can’t complete
- All cargo is picked up, loaded, and delivered in real time
- Vehicles are cleaned up on cancel or disconnect
- Cooldown system per player

### 🎯 Target + UI
- Compatible with `ox_target`, `qb-target`, or fallback to 3D Text
- Uses `ox_lib` context menus and progress circles
- Clean UI dialogs with job confirmation, mission summary & alerts

---

## 🛠️ Requirements

You **must have**:

- `ox_lib`
- `qbx_core` (or `qb-core`)
- One of:
  - `ox_target` ✅ recommended
  - `qb-target`
  - None (fallback available)

Optional support:

- `ps-dispatch`, `cd_dispatch`, or your own custom dispatch
- Fuel systems:
  - `ox_fuel`
  - `ps-fuel`
  - `cdn-fuel`
  - `lc_fuel`
- Keys systems:
  - `qb-vehiclekeys`
  - `cd_garage`
  - `wasabi_carlock`

---

## ⚙️ Configuration

Edit `config.lua` to adjust:

- Target system: `Config.Target = 'ox_target'` (or `qb-target`, or `none`)
- Dispatch system: `Config.Dispatch = 'ps-dispatch'` (or `cd_dispatch`, or `custom`)
- Payment amounts, enemy difficulty, cooldown times
- Truck spawn locations, blip icons, models, fuel levels, and more

---

## 🚨 PS-Dispatch Setup

To integrate with **ps-dispatch**, follow these steps:

### 1. Add this to your `ps-dispatch/config.lua` inside `Config.Alerts`:
```lua
['trucking_heist'] = {
    radius = 0,
    sprite = 161,
    color = 1,
    scale = 1.5,
    length = 5, -- 5 minutes
    sound = 'Lose_1st',
    sound2 = 'GTAO_FM_Events_Soundset',
    offset = false,
    flash = false
}

2. Add this to your ps-dispatch/locales/en.lua:
lua
Copy
Edit
['trucking_heist'] = 'Suspicious Trucking Activity'
3. Set the dispatch type in your filthy_truckerjob/config.lua:
lua
Copy
Edit
Config.Dispatch = 'ps-dispatch'
🔧 Installation
🗂️ Drag & Drop
Place the entire filthy_truckerjob folder into your resources folder.

📜 Ensure Dependencies
Make sure the following are started before this script:

bash
Copy
Edit
ensure ox_lib
ensure qbx_core -- or qb-core
ensure filthy_truckerjob
🛠️ Configure (Optional)
Open config.lua and:

Set your framework (qbox or qbcore)

Choose your target, dispatch, keys, and fuel systems

Customize notification slang 🇿🇦 (e.g. "Awu jita! You collected a box!")

✅ You're Done!
restart your server or use:
/ensure filthy_truckerjob

Then head to Mr. Mkize (blip 477), and get hustling. Legal or illegal, you decide. 😏
Jobs include progress tracking, risk, payout scaling, and cop alerts — perfect for immersive trucking roleplay.

If you run into issues, join our support server: 👉 https://discord.gg/FDKudWACcQ
Dankie for installing! May your trailers stay attached and your boxes stay stacked. 🇿🇦🛻🔥
