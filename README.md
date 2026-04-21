# Glogger
The Gorgon Log parsing app by Zenith of Dreva.

- Thanks Reyetta, Wogan, Kaeus, Fidge, TwinkleofToes, DisasterGaymer, Cakedydidooda, Lucyfeir and Deradon! Feedback and early testing was super helpful in getting Glogger to where it is now. :D
- Some things only will work with VIP! This is just a limitation of how and where I can access data. The DataBrowser works no matter what though, and it is a very handy. Nothing in here is intentionally broken because of non-vip. I just can only work with what I have.
- It operates on the Player.log, ChatLogs, and the CDN data provided by Citan for app developers. (Thanks Citan!) No shady poking in to running processes or anything like that.
- There is no server for this app to talk to; everything runs locally to try and keep it as speedy and responsive as possible. Has to download some Citan-provided data on boot and with new patches, and pokes github to check for app updates.

I apologize for bad UI/UX/programming - I'm a game designer by trade, not a software engineer. I'm more at home with excel and scripts than app development, so I'm learning as I go.

## Why beta?

- We still don't have 100% capture rate on items going in/out of inventory sometimes. It is a stubborn bug, and I'm trying to track it down. It is pretty dang good, but not 100%
- There is a lot of UI/UX inconsistencies that I just haven't rooted out yet.
- Lots of little leftover minor bugs to fix here and there.
- A few key features I want to implement before it feels whole.
- but the biggest issue is _no documentation_ so far! It very much is in a "play with it and figure it out" state, and a lot of the screens _really_ need some guidance to tell you how to use them.

## Initial Setup

1. Go to your VIP settings, export your character and storage JSONs. (If you've got alts, it is helpful to do them as well!)
<img width="1344" height="1170" alt="image" src="https://github.com/user-attachments/assets/5b164e75-6b18-4d7e-b195-3e98108f8de9" />

2. Turn on the chat logging! This will give you a chat history browser and allow you to set watchwords! Also turning on combat logging doesn't do a ton, but does allow you to see death reports on what killed you. (I have no plans to try to make DPS meters or anything.)
<img width="979" height="976" alt="image" src="https://github.com/user-attachments/assets/a49801b1-8d41-4fb8-b32e-70ca0a5a5d9c" />

3. Turn on book mode; this helps with a handful of features.
<img width="983" height="403" alt="image" src="https://github.com/user-attachments/assets/5304ec78-a4b3-41c7-b6fa-9693201090f9" />

4. Start Glogger! The setup wizard should walk you through the very fast setup with hopefully minimal issues. 
<img width="752" height="604" alt="image" src="https://github.com/user-attachments/assets/7a3007cb-34c1-4315-9d92-6024e3b50824" />
<img width="697" height="554" alt="image" src="https://github.com/user-attachments/assets/58f23b7c-cb90-44c8-95cd-d77512863188" />
<img width="625" height="942" alt="image" src="https://github.com/user-attachments/assets/7a59c803-85c8-4051-b80f-a10047a82499" />

## Feature Screenshots

### Dashboard Screen w/Widgets
Several widgets can be toggled on/off to provide (hopefully) useful information. Some customization. 
<img width="2537" height="1346" alt="image" src="https://github.com/user-attachments/assets/42895f1c-8413-4d8d-9c2c-104a685a9a72" />

### Character Stats Page
We pull in `/behaviorreport/` and `/age` and combine it with exported JSONs and parsed Player.log ability updates to make a page full of numbers. Usefulness TBD, but numbers.
<img width="2537" height="1357" alt="image" src="https://github.com/user-attachments/assets/fc9c2bbf-6847-4161-8629-2b6ffb2eb946" />
Also, we tell you the cursed stat:
<img width="797" height="26" alt="image" src="https://github.com/user-attachments/assets/2e29fb73-cd7c-4038-8d24-a5d3c1cb9dd9" />

### NPC Details
As much information as I can reasonably fit. See shop spend cap increases, storage increases, feature unlocks, gift info, and training.
<img width="2548" height="1343" alt="image" src="https://github.com/user-attachments/assets/4735c8a3-807a-4bb7-ae7f-e6e24848bcd8" />

### Deaths Tracker
If you're curious what killed you, now you can learn! It takes some time to backfill the damage info for abilities prior to the lethal one, but it gives you an idea what has been murdering you.
<img width="2540" height="1350" alt="image" src="https://github.com/user-attachments/assets/3323cf7b-730f-451e-a728-319c7f4b3383" />

### Gourmand Report
See what you have eaten and what you need to eat! Also figure out what your favorite foods are.
<img width="1532" height="1225" alt="image" src="https://github.com/user-attachments/assets/d13ceba9-f5fd-4af0-b4b9-ec047eb8679d" />

### Statehelm Gift Tracker
It tracks statehelm gifts! Soon to come: weekly quest tracking, too.
<img width="2514" height="1256" alt="image" src="https://github.com/user-attachments/assets/0135bcdd-ccd0-456d-b2aa-006ef6e1a870" />

### Build Planner
A fully-fledged build planner with crafting point support.
<img width="2552" height="1334" alt="image" src="https://github.com/user-attachments/assets/cd0a2ddc-7993-4f6f-b3ab-613126798faa" />

### Crafting Projects
Plan your crafting project, see where your materials are, decide to craft or buy intermediates. 
<img width="2552" height="1362" alt="image" src="https://github.com/user-attachments/assets/411979ba-f2d8-45f8-a956-4912416670f9" />

### Craft Skill Report
See exactly how many materials and the estimated value of those materials you've throw in to the endless money pit of crafting!
<img width="2529" height="1246" alt="image" src="https://github.com/user-attachments/assets/55d0b6ab-8249-4d8e-876e-13c2da79cfde" />

### Surveying Tracker
Session-by-session survey tracking. Also an analytics page to compile all your data by zone, globally, or by survey type!
<img width="2552" height="1388" alt="image" src="https://github.com/user-attachments/assets/a44a8505-f6ff-4a73-8bab-4a6a10d2f76e" />
<img width="2548" height="1354" alt="image" src="https://github.com/user-attachments/assets/85f94aaa-a3b5-44e3-bd1c-70dae96900f2" />

### Stall Tracker
Open up your daily reports to have Glogger ingest them and provide a historical view of your stall!
<img width="2553" height="1347" alt="image" src="https://github.com/user-attachments/assets/40845bbf-4fdf-46ab-b80a-4e8f349141f9" />

### Chat Logs
Chat logs with item links, full searchability (including 'from:' and 'in:') along with watchwords that highlights key words, items, or users across all your channels.
<img width="2546" height="1363" alt="image" src="https://github.com/user-attachments/assets/9d0969be-c2b8-498b-881c-1779825177ec" />
<img width="2547" height="1358" alt="image" src="https://github.com/user-attachments/assets/ed946002-52c5-4336-a32d-14bf97595bc2" />

### Data Browser
A fully functional, searchable data browser of the CDN data. Cross-linked and referenced. It's like a snappy, locally-run wiki! Just without a bunch of the useful player-written information. Also supports diffing between prior game version and current!
<img width="2520" height="1330" alt="image" src="https://github.com/user-attachments/assets/5634ace0-3bce-4998-af0b-67325087fe47" />

### And more!
...auto record words of power, cook all the food your friend is missing for gourmand, track your brewing recipes discovered, plan your crafting levelling, configure what items are used for dynamic recipes, set market data on item tooltips, pin tooltips to the bottom for quick reference, and probably other stuff i'm forgetting!


