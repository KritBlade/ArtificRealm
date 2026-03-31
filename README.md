# ArtificRealm

> **SillyTavern Character Card** — License GPL 3.0, **NOT** for commercial use.

## 🎮 Regular Player

I am releasing the MVU Zod Character card **Artific Realm (アーティフィック レルム 創世域)**. 
* 📺 **[Installation Video Guide](https://youtu.be/Jh1ojfiqGXI)** (All required extension links are in the video description).
* 📥 **[Download Release Here](https://github.com/KritBlade/ArtificRealm/releases/)**

**Important:** You are required to follow the YouTube video above to install the necessary extensions, or the card will not work. Playing on a PC is highly recommended due to the large interface.

### The World
This character card drops you into an *Isekai* world filled with magic, dwarves, elves, demons, fairies, and more. A powerful suction drags you—the main character—into this world. Upon arrival, you are supercharged with four exclusive plugins:

* **[Soul Covenant]** - Can bind female characters as Familiars.
* **[Inventory]** - A four-dimensional space that can store any small non-living objects (items, clothes, food, etc.).
* **[System Panel]** - An RPG game-like display panel visible only to you. It shows targets' basic stats alongside surface and hidden personality traits.
* **[Phoenix Pact]** - Allows the player to actively record the current point in time as a "Save Point".

> *When you wake up inside a damaged wooden hut, a nun called Engni is staring at you nervously...*

### NSFW & Gameplay Note
This is a NSFW game, but you do **NOT** need to play NSFW if you don't want to; it is not hardcoded to be overly explicit. Unlike other RPG NSFW games, all of the Heroines ($\color{red}{\text{16 of them}}$) inside the game have serious personality flaws. As the main character, you must learn their flaws and use them to your advantage to survive in the Isekai world. These flaws can be deadly towards enemies if utilized correctly.

---

## ⚙️ Installation

It will take about 6 minutes to [install the extensions](https://youtu.be/Jh1ojfiqGXI) correctly for SillyTavern. This guide assumes you already have a working connection to an AI service provider.

This card heavily utilizes the **Tavern Helper** extension, which enables JavaScript in the SillyTavern engine. This allows for persistent data in your story! Every stat in the status menu is saved locally on your hard drive, meaning the AI does *not* need to remember these stats or keep track of states in its context.

### Recommended AI Models
You will need a highly capable AI to pull this off:
* **Great:** Gemini Flash 3.0 preview, Gemini 2.5, Gemini 3.0/3.1 Pro, most Claude models.
* **Okay:** Kimi 2.5 (works, but processing takes a long time).
* **Not Recommended:** Deepseek 3.2 (struggles to hide the `<think>` process), and most lower-end models (stat updates may fail).

### Presets
Because the game requires a preset that works with Tavern Helper, most standard Western presets won't update the stats correctly. 
* **[Izumi Preset](https://discord.gg/C6HabNwzn7)**: Found inside the linked Discord channel (has some English translation).
* **[Megumin Preset](https://www.reddit.com/r/SillyTavernAI/comments/1s2pfj6/megumin_suite_v41_dev_mode_and_bug_fixes/)**: A Reddit alternative that also works fine. Follow their instructions to install the extension and preset.

<div align="center">
  <img width="800" alt="Izumi Preset Example" src="https://github.com/user-attachments/assets/71af5433-4ef1-4d0f-9e60-207462bc71f0" />
</div>

Once in the game, you can view the stat storage in JSON format from the Variable Manager. You can view every single floor of the chat here and modify stats directly if needed. The Prompt Viewer allows you to see the exact prompt sent to the AI (highly useful for preset builders).

<div align="center">
  <img height="450" alt="Variable Manager 1" src="https://github.com/user-attachments/assets/c564ca7b-b0d5-4073-aa8d-0fcb70ef5ec2" />
  <img height="500" alt="Variable Manager 2" src="https://github.com/user-attachments/assets/3240e667-95a6-452b-a9bd-a5d8f4a98e2f" />
</div>

---

## 📜 Credits & Lore

Credit where credit is due:
* **World Lore:** Loosely based on *"The Fallen Psalms of Terrarien"*. The lorebook was massive, so I kept it as-is and translated it into English.
* **Character Design:** Inspired by *"Building a Harem in an Otherworld Full of Villainous Bitches"*.

*Note on Translation:* The most difficult part of this project was translating while keeping names consistent. You will still see AI translation quirks here and there, but correcting all of them is too massive an effort.

---

## 🛠️ Preset Builder

As shown in the video, players must download a preset for MVU variable updates to work correctly. I hope someone in the community eventually builds a fully English preset for Tavern Helper with MVU Zod support!

The main challenge isn't adding bells and whistles—it's squeezing the minimum required features while keeping output tokens small. The [Izumi preset](https://discord.gg/C6HabNwzn7) works well and includes a quest number generator (great for JSONpatch into MVU variables). It features this MVU update structure:

```xml
<UpdateVariable>
  <Analysis>
  </Analysis>
  <JSONPatch>
  </JSONPatch>
</UpdateVariable>
