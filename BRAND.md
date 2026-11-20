<!-- @format -->

<p align="center">
  <img src="./brand/banners/banner-purple.svg" alt="Xernerx Studios Official Banner" width="100%" />
</p>

<h1 align="center">Xernerx Studios — Official Brand &amp; Press Kit</h1>

<p align="center">
  <b>1 Account, 1 Place, 1 Setup</b><br />
  Official brand guidelines, typography specifications, 27-color palette tokens, logos, icons, banners, and SDK media assets for <b>Xernerx Studios</b>.
</p>

<p align="center">
  <a href="./brand/brand.json"><img src="https://img.shields.io/badge/Manifest-brand.json-8b7cf6?style=for-the-badge" alt="Brand JSON Manifest" /></a>
  <a href="https://www.xernerx.com"><img src="https://img.shields.io/badge/Website-xernerx.com-6366f1?style=for-the-badge" alt="Website" /></a>
  <a href="https://docs.xernerx.com/packages"><img src="https://img.shields.io/badge/SDK_Docs-docs.xernerx.com-06b6d4?style=for-the-badge" alt="Documentation" /></a>
</p>

---

## 📑 Table of Contents

1. [Core Brand Identity](#-core-brand-identity)
2. [Official Typography](#-official-typography)
3. [Primary Brand Marks (Logos, Icons & Banners)](#-primary-brand-marks-logos-icons--banners)
4. [Core Surface & Theme Tokens](#-core-surface--theme-tokens)
5. [Official 27-Color Xernerx Palette](#-official-27-color-xernerx-palette)
6. [Official Discord Applications Media Kit (`Virtue`, `YourApps`, `TDL`, `Zodiac` & `Metamorphosis`)](#-official-discord-applications-media-kit-virtue-yourapps-tdl-zodiac--metamorphosis)
7. [Official SDK Package Media Kit (`@xernerx/*`)](#-official-sdk-package-media-kit-xernerx)
8. [Brand Usage Guidelines](#-brand-usage-guidelines)

---

## 🏛️ Core Brand Identity

- **Organization Name:** `Xernerx Studios` (short form: `Xernerx`)
- **Platform Suite Name:** `Xernerx Suite`
- **Official Slogan:** `1 Account, 1 Place, 1 Setup`
- **Signature Brand Color:** **Xernerx Purple** (`#8b7cf6` / `rgb(139, 124, 246)`)
- **Machine-Readable Manifest:** [`./brand/brand.json`](./brand/brand.json) (also hosted at [`https://www.xernerx.com/brand.json`](https://www.xernerx.com/brand.json))
- **UI & Component Design System Specification:** [`../suite/DESIGN.md`](../suite/DESIGN.md) (*Modern Round Glassmorphism Pop*, Tailwind CSS v4 tokens, geometry, and `@xernerx/ui` primitives)

---

## 🔤 Official Typography

All **Xernerx Suite** web applications, desktop clients, and developer portals use two official open-source typefaces loaded via Google Fonts and exposed through [`@xernerx/styles`](https://github.com/Xernerx):

| Role | Typeface | CSS Variable | Weights | Fallback Stack | Download / Specimen |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Primary UI, Headings & Display** | **Fredoka** | `--font-fredoka` | `300`, `400`, `500`, `600`, `700` | `system-ui, -apple-system, sans-serif` | [Google Fonts: Fredoka](https://fonts.google.com/specimen/Fredoka) |
| **Monospace, Code, CLI & Keybinds** | **Cascadia Code** | `--font-cascadia` | `400`, `600`, `700` | `ui-monospace, SFMono-Regular, Menlo, monospace` | [Google Fonts: Cascadia Code](https://fonts.google.com/specimen/Cascadia+Code) |

### CSS Implementation

```css
@import url('https://fonts.googleapis.com/css2?family=Cascadia+Code:wght@400..700&family=Fredoka:wght@300..700&display=swap');

:root {
	--font-fredoka: 'Fredoka', system-ui, -apple-system, sans-serif;
	--font-cascadia: 'Cascadia Code', ui-monospace, SFMono-Regular, Menlo, monospace;
}

body {
	font-family: var(--font-fredoka);
}

code,
pre,
kbd {
	font-family: var(--font-cascadia);
}
```

---

## 🛡️ Primary Brand Marks (Logos, Icons & Banners)

Xernerx Studios uses three primary brand marks. Vector `.svg` files in [`./brand/`](./brand) include both `currentColor` adaptive templates (`logo.svg`, `icon.svg`, `banner.svg`) and pre-colored variants across all 27 official Xernerx colors.

| Mark | Preview | Dimensions | Formats | Primary Use Case | Default Downloads |
| :--- | :---: | :---: | :---: | :--- | :--- |
| **Xernerx Winged Crest (`logo`)** | <img src="./brand/logos/logo-purple.svg" alt="Xernerx Crest Logo" width="64" height="64" /> | `1250 × 1250` | `.svg`, `.png` | Transparent standalone crest for headers, watermarks, hero graphics, and partner badges. | [SVG (`currentColor`)](./brand/logos/logo.svg) · [SVG (`purple`)](./brand/logos/logo-purple.svg) · [PNG](./brand/logos/logo.png) |
| **Xernerx App Badge (`icon`)** | <img src="./brand/icons/icon-purple.svg" alt="Xernerx App Icon" width="64" height="64" /> | `870 × 870` | `.svg`, `.png`, `.ico` | Circular badge (`#191a1e` dark surface fill) for app icons, avatars, favicons, and desktop shortcuts. | [SVG (`currentColor`)](./brand/icons/icon.svg) · [SVG (`purple`)](./brand/icons/icon-purple.svg) · [PNG](./brand/icons/icon.png) · [ICO](./brand/icons/icon.ico) |
| **Xernerx Wordmark (`banner`)** | <img src="./brand/banners/banner-purple.svg" alt="Xernerx Wordmark Banner" width="220" /> | `2000 × 990` | `.svg`, `.png` | Full horizontal winged crest + `xernerx` wordmark for repository headers, OpenGraph cards, and press headers. | [SVG (`currentColor`)](./brand/banners/banner.svg) · [SVG (`purple`)](./brand/banners/banner-purple.svg) · [PNG](./brand/banners/banner.png) |
| **Environment Wordmarks (`canary` / `dev`)** | <img src="./brand/banners/banner-canary.svg" alt="Xernerx Canary Banner" width="220" /> | `2000 × 500` | `.svg` | Official environment indicator banners for `.canary.xernerx.com` and `.dev.xernerx.com`. | [Canary SVG](./brand/banners/banner-canary.svg) · [Dev SVG](./brand/banners/banner-dev.svg) |

---

## 🌗 Core Surface & Theme Tokens

These surface tokens define the dark and light theme foundations in `@xernerx/styles`:

| Swatch | Token Name | CSS Variable | Hex | RGB | Usage |
| :---: | :--- | :--- | :--- | :--- | :--- |
| <img src="./brand/swatches/bg-dark.svg" width="20" height="20" alt="#09090b" /> | **Background (Dark)** | `--background-dark` | `#09090b` | `rgb(9, 9, 11)` | Primary app canvas in Dark Mode |
| <img src="./brand/swatches/fg-dark.svg" width="20" height="20" alt="#18181b" /> | **Foreground / Card (Dark)** | `--foreground-dark` | `#18181b` | `rgb(24, 24, 27)` | Elevated cards, panels, and modals in Dark Mode |
| <img src="./brand/swatches/badge-dark.svg" width="20" height="20" alt="#191a1e" /> | **Icon Badge Surface (Dark)** | *Icon disc fill* | `#191a1e` | `rgb(25, 26, 30)` | Circular badge background on `icon-*.svg` |
| <img src="./brand/swatches/border-dark.svg" width="20" height="20" alt="#f4f4f5" /> | **Border (Dark)** | `--border-dark` | `#f4f4f5` | `rgb(244, 244, 245)` | Subtle structural borders (with opacity modifiers) |
| <img src="./brand/swatches/text-dark.svg" width="20" height="20" alt="#fafafa" /> | **Primary Text (Dark)** | `--text` | `#fafafa` | `rgb(250, 250, 250)` | Primary body & heading text in Dark Mode |
| <img src="./brand/swatches/text-muted-dark.svg" width="20" height="20" alt="#a1a1aa" /> | **Muted Text (Dark)** | `--text-muted` | `#a1a1aa` | `rgb(161, 161, 170)` | Secondary labels & metadata in Dark Mode |
| <img src="./brand/swatches/bg-light.svg" width="20" height="20" alt="#fafafa" /> | **Background (Light)** | `--background-light` | `#fafafa` | `rgb(250, 250, 250)` | Primary app canvas in Light Mode |
| <img src="./brand/swatches/fg-light.svg" width="20" height="20" alt="#f4f4f5" /> | **Foreground / Card (Light)** | `--foreground-light` | `#f4f4f5` | `rgb(244, 244, 245)` | Elevated cards, panels, and Light Mode icon disc fill |
| <img src="./brand/swatches/border-light.svg" width="20" height="20" alt="#53535b" /> | **Border (Light)** | `--border-light` | `#53535b` | `rgb(83, 83, 91)` | Subtle structural borders in Light Mode |
| <img src="./brand/swatches/text-light.svg" width="20" height="20" alt="#09090b" /> | **Primary Text (Light)** | `--text` | `#09090b` | `rgb(9, 9, 11)` | Primary body & heading text in Light Mode |
| <img src="./brand/swatches/text-muted-light.svg" width="20" height="20" alt="#52525b" /> | **Muted Text (Light)** | `--text-muted` | `#52525b` | `rgb(82, 82, 91)` | Secondary labels & metadata in Light Mode |

---

## 🎨 Official 27-Color Xernerx Palette

Every official Xernerx accent color has pre-rendered **Crest Logos** (`1250×1250`), **App Icons** (`870×870` + multi-size `.ico`), and **Wordmark Banners** (`2000×990`) available in both [`./brand/`](./brand) and across all `*.xernerx.com` origins:

| Swatch | Icon | Color Name | Key | Hex | RGB | Crest Logo (`1250×1250`) | App Icon (`870×870`) | Wordmark Banner (`2000×990`) |
| :---: | :---: | :--- | :--- | :--- | :--- | :---: | :---: | :---: |
| <img src="./brand/swatches/purple.svg" width="20" height="20" /> | <img src="./brand/icons/icon-purple.svg" width="28" height="28" /> | **Purple** *(Default)* | `purple` | `#8b7cf6` | `rgb(139, 124, 246)` | [SVG](./brand/logos/logo-purple.svg) · [PNG](./brand/logos/logo-purple.png) | [SVG](./brand/icons/icon-purple.svg) · [PNG](./brand/icons/icon-purple.png) · [ICO](./brand/icons/icon-purple.ico) | [SVG](./brand/banners/banner-purple.svg) · [PNG](./brand/banners/banner-purple.png) |
| <img src="./brand/swatches/violet.svg" width="20" height="20" /> | <img src="./brand/icons/icon-violet.svg" width="28" height="28" /> | **Violet** | `violet` | `#7c3aed` | `rgb(124, 58, 237)` | [SVG](./brand/logos/logo-violet.svg) · [PNG](./brand/logos/logo-violet.png) | [SVG](./brand/icons/icon-violet.svg) · [PNG](./brand/icons/icon-violet.png) · [ICO](./brand/icons/icon-violet.ico) | [SVG](./brand/banners/banner-violet.svg) · [PNG](./brand/banners/banner-violet.png) |
| <img src="./brand/swatches/indigo.svg" width="20" height="20" /> | <img src="./brand/icons/icon-indigo.svg" width="28" height="28" /> | **Indigo** | `indigo` | `#6366f1` | `rgb(99, 102, 241)` | [SVG](./brand/logos/logo-indigo.svg) · [PNG](./brand/logos/logo-indigo.png) | [SVG](./brand/icons/icon-indigo.svg) · [PNG](./brand/icons/icon-indigo.png) · [ICO](./brand/icons/icon-indigo.ico) | [SVG](./brand/banners/banner-indigo.svg) · [PNG](./brand/banners/banner-indigo.png) |
| <img src="./brand/swatches/cobalt.svg" width="20" height="20" /> | <img src="./brand/icons/icon-cobalt.svg" width="28" height="28" /> | **Cobalt** | `cobalt` | `#2563eb` | `rgb(37, 99, 235)` | [SVG](./brand/logos/logo-cobalt.svg) · [PNG](./brand/logos/logo-cobalt.png) | [SVG](./brand/icons/icon-cobalt.svg) · [PNG](./brand/icons/icon-cobalt.png) · [ICO](./brand/icons/icon-cobalt.ico) | [SVG](./brand/banners/banner-cobalt.svg) · [PNG](./brand/banners/banner-cobalt.png) |
| <img src="./brand/swatches/blue.svg" width="20" height="20" /> | <img src="./brand/icons/icon-blue.svg" width="28" height="28" /> | **Blue** | `blue` | `#3b82f6` | `rgb(59, 130, 246)` | [SVG](./brand/logos/logo-blue.svg) · [PNG](./brand/logos/logo-blue.png) | [SVG](./brand/icons/icon-blue.svg) · [PNG](./brand/icons/icon-blue.png) · [ICO](./brand/icons/icon-blue.ico) | [SVG](./brand/banners/banner-blue.svg) · [PNG](./brand/banners/banner-blue.png) |
| <img src="./brand/swatches/sky.svg" width="20" height="20" /> | <img src="./brand/icons/icon-sky.svg" width="28" height="28" /> | **Sky** | `sky` | `#38bdf8` | `rgb(56, 189, 248)` | [SVG](./brand/logos/logo-sky.svg) · [PNG](./brand/logos/logo-sky.png) | [SVG](./brand/icons/icon-sky.svg) · [PNG](./brand/icons/icon-sky.png) · [ICO](./brand/icons/icon-sky.ico) | [SVG](./brand/banners/banner-sky.svg) · [PNG](./brand/banners/banner-sky.png) |
| <img src="./brand/swatches/cyan.svg" width="20" height="20" /> | <img src="./brand/icons/icon-cyan.svg" width="28" height="28" /> | **Cyan** | `cyan` | `#06b6d4` | `rgb(6, 182, 212)` | [SVG](./brand/logos/logo-cyan.svg) · [PNG](./brand/logos/logo-cyan.png) | [SVG](./brand/icons/icon-cyan.svg) · [PNG](./brand/icons/icon-cyan.png) · [ICO](./brand/icons/icon-cyan.ico) | [SVG](./brand/banners/banner-cyan.svg) · [PNG](./brand/banners/banner-cyan.png) |
| <img src="./brand/swatches/mint.svg" width="20" height="20" /> | <img src="./brand/icons/icon-mint.svg" width="28" height="28" /> | **Mint** | `mint` | `#2dd4bf` | `rgb(45, 212, 191)` | [SVG](./brand/logos/logo-mint.svg) · [PNG](./brand/logos/logo-mint.png) | [SVG](./brand/icons/icon-mint.svg) · [PNG](./brand/icons/icon-mint.png) · [ICO](./brand/icons/icon-mint.ico) | [SVG](./brand/banners/banner-mint.svg) · [PNG](./brand/banners/banner-mint.png) |
| <img src="./brand/swatches/emerald.svg" width="20" height="20" /> | <img src="./brand/icons/icon-emerald.svg" width="28" height="28" /> | **Emerald** | `emerald` | `#10b981` | `rgb(16, 185, 129)` | [SVG](./brand/logos/logo-emerald.svg) · [PNG](./brand/logos/logo-emerald.png) | [SVG](./brand/icons/icon-emerald.svg) · [PNG](./brand/icons/icon-emerald.png) · [ICO](./brand/icons/icon-emerald.ico) | [SVG](./brand/banners/banner-emerald.svg) · [PNG](./brand/banners/banner-emerald.png) |
| <img src="./brand/swatches/green.svg" width="20" height="20" /> | <img src="./brand/icons/icon-green.svg" width="28" height="28" /> | **Green** | `green` | `#a4b795` | `rgb(164, 183, 149)` | [SVG](./brand/logos/logo-green.svg) · [PNG](./brand/logos/logo-green.png) | [SVG](./brand/icons/icon-green.svg) · [PNG](./brand/icons/icon-green.png) · [ICO](./brand/icons/icon-green.ico) | [SVG](./brand/banners/banner-green.svg) · [PNG](./brand/banners/banner-green.png) |
| <img src="./brand/swatches/neon.svg" width="20" height="20" /> | <img src="./brand/icons/icon-neon.svg" width="28" height="28" /> | **Neon** | `neon` | `#39ff14` | `rgb(57, 255, 20)` | [SVG](./brand/logos/logo-neon.svg) · [PNG](./brand/logos/logo-neon.png) | [SVG](./brand/icons/icon-neon.svg) · [PNG](./brand/icons/icon-neon.png) · [ICO](./brand/icons/icon-neon.ico) | [SVG](./brand/banners/banner-neon.svg) · [PNG](./brand/banners/banner-neon.png) |
| <img src="./brand/swatches/lime.svg" width="20" height="20" /> | <img src="./brand/icons/icon-lime.svg" width="28" height="28" /> | **Lime** | `lime` | `#acc813` | `rgb(172, 200, 19)` | [SVG](./brand/logos/logo-lime.svg) · [PNG](./brand/logos/logo-lime.png) | [SVG](./brand/icons/icon-lime.svg) · [PNG](./brand/icons/icon-lime.png) · [ICO](./brand/icons/icon-lime.ico) | [SVG](./brand/banners/banner-lime.svg) · [PNG](./brand/banners/banner-lime.png) |
| <img src="./brand/swatches/yellow.svg" width="20" height="20" /> | <img src="./brand/icons/icon-yellow.svg" width="28" height="28" /> | **Yellow** | `yellow` | `#eab308` | `rgb(234, 179, 8)` | [SVG](./brand/logos/logo-yellow.svg) · [PNG](./brand/logos/logo-yellow.png) | [SVG](./brand/icons/icon-yellow.svg) · [PNG](./brand/icons/icon-yellow.png) · [ICO](./brand/icons/icon-yellow.ico) | [SVG](./brand/banners/banner-yellow.svg) · [PNG](./brand/banners/banner-yellow.png) |
| <img src="./brand/swatches/gold.svg" width="20" height="20" /> | <img src="./brand/icons/icon-gold.svg" width="28" height="28" /> | **Gold** | `gold` | `#f59e0b` | `rgb(245, 158, 11)` | [SVG](./brand/logos/logo-gold.svg) · [PNG](./brand/logos/logo-gold.png) | [SVG](./brand/icons/icon-gold.svg) · [PNG](./brand/icons/icon-gold.png) · [ICO](./brand/icons/icon-gold.ico) | [SVG](./brand/banners/banner-gold.svg) · [PNG](./brand/banners/banner-gold.png) |
| <img src="./brand/swatches/orange.svg" width="20" height="20" /> | <img src="./brand/icons/icon-orange.svg" width="28" height="28" /> | **Orange** | `orange` | `#f97316` | `rgb(249, 115, 22)` | [SVG](./brand/logos/logo-orange.svg) · [PNG](./brand/logos/logo-orange.png) | [SVG](./brand/icons/icon-orange.svg) · [PNG](./brand/icons/icon-orange.png) · [ICO](./brand/icons/icon-orange.ico) | [SVG](./brand/banners/banner-orange.svg) · [PNG](./brand/banners/banner-orange.png) |
| <img src="./brand/swatches/peach.svg" width="20" height="20" /> | <img src="./brand/icons/icon-peach.svg" width="28" height="28" /> | **Peach** | `peach` | `#fdba74` | `rgb(253, 186, 116)` | [SVG](./brand/logos/logo-peach.svg) · [PNG](./brand/logos/logo-peach.png) | [SVG](./brand/icons/icon-peach.svg) · [PNG](./brand/icons/icon-peach.png) · [ICO](./brand/icons/icon-peach.ico) | [SVG](./brand/banners/banner-peach.svg) · [PNG](./brand/banners/banner-peach.png) |
| <img src="./brand/swatches/coral.svg" width="20" height="20" /> | <img src="./brand/icons/icon-coral.svg" width="28" height="28" /> | **Coral** | `coral` | `#fb7185` | `rgb(251, 113, 133)` | [SVG](./brand/logos/logo-coral.svg) · [PNG](./brand/logos/logo-coral.png) | [SVG](./brand/icons/icon-coral.svg) · [PNG](./brand/icons/icon-coral.png) · [ICO](./brand/icons/icon-coral.ico) | [SVG](./brand/banners/banner-coral.svg) · [PNG](./brand/banners/banner-coral.png) |
| <img src="./brand/swatches/crimson.svg" width="20" height="20" /> | <img src="./brand/icons/icon-crimson.svg" width="28" height="28" /> | **Crimson** | `crimson` | `#ef4444` | `rgb(239, 68, 68)` | [SVG](./brand/logos/logo-crimson.svg) · [PNG](./brand/logos/logo-crimson.png) | [SVG](./brand/icons/icon-crimson.svg) · [PNG](./brand/icons/icon-crimson.png) · [ICO](./brand/icons/icon-crimson.ico) | [SVG](./brand/banners/banner-crimson.svg) · [PNG](./brand/banners/banner-crimson.png) |
| <img src="./brand/swatches/red.svg" width="20" height="20" /> | <img src="./brand/icons/icon-red.svg" width="28" height="28" /> | **Red** | `red` | `#ef4444` | `rgb(239, 68, 68)` | [SVG](./brand/logos/logo-red.svg) · [PNG](./brand/logos/logo-red.png) | [SVG](./brand/icons/icon-red.svg) · [PNG](./brand/icons/icon-red.png) · [ICO](./brand/icons/icon-red.ico) | [SVG](./brand/banners/banner-red.svg) · [PNG](./brand/banners/banner-red.png) |
| <img src="./brand/swatches/berry.svg" width="20" height="20" /> | <img src="./brand/icons/icon-berry.svg" width="28" height="28" /> | **Berry** | `berry` | `#e11d48` | `rgb(225, 29, 72)` | [SVG](./brand/logos/logo-berry.svg) · [PNG](./brand/logos/logo-berry.png) | [SVG](./brand/icons/icon-berry.svg) · [PNG](./brand/icons/icon-berry.png) · [ICO](./brand/icons/icon-berry.ico) | [SVG](./brand/banners/banner-berry.svg) · [PNG](./brand/banners/banner-berry.png) |
| <img src="./brand/swatches/pink.svg" width="20" height="20" /> | <img src="./brand/icons/icon-pink.svg" width="28" height="28" /> | **Pink** | `pink` | `#ec4899` | `rgb(236, 72, 153)` | [SVG](./brand/logos/logo-pink.svg) · [PNG](./brand/logos/logo-pink.png) | [SVG](./brand/icons/icon-pink.svg) · [PNG](./brand/icons/icon-pink.png) · [ICO](./brand/icons/icon-pink.ico) | [SVG](./brand/banners/banner-pink.svg) · [PNG](./brand/banners/banner-pink.png) |
| <img src="./brand/swatches/magenta.svg" width="20" height="20" /> | <img src="./brand/icons/icon-magenta.svg" width="28" height="28" /> | **Magenta** | `magenta` | `#d946ef` | `rgb(217, 70, 239)` | [SVG](./brand/logos/logo-magenta.svg) · [PNG](./brand/logos/logo-magenta.png) | [SVG](./brand/icons/icon-magenta.svg) · [PNG](./brand/icons/icon-magenta.png) · [ICO](./brand/icons/icon-magenta.ico) | [SVG](./brand/banners/banner-magenta.svg) · [PNG](./brand/banners/banner-magenta.png) |
| <img src="./brand/swatches/lavender.svg" width="20" height="20" /> | <img src="./brand/icons/icon-lavender.svg" width="28" height="28" /> | **Lavender** | `lavender` | `#c084fc` | `rgb(192, 132, 252)` | [SVG](./brand/logos/logo-lavender.svg) · [PNG](./brand/logos/logo-lavender.png) | [SVG](./brand/icons/icon-lavender.svg) · [PNG](./brand/icons/icon-lavender.png) · [ICO](./brand/icons/icon-lavender.ico) | [SVG](./brand/banners/banner-lavender.svg) · [PNG](./brand/banners/banner-lavender.png) |
| <img src="./brand/swatches/slate.svg" width="20" height="20" /> | <img src="./brand/icons/icon-slate.svg" width="28" height="28" /> | **Slate** | `slate` | `#64748b` | `rgb(100, 116, 139)` | [SVG](./brand/logos/logo-slate.svg) · [PNG](./brand/logos/logo-slate.png) | [SVG](./brand/icons/icon-slate.svg) · [PNG](./brand/icons/icon-slate.png) · [ICO](./brand/icons/icon-slate.ico) | [SVG](./brand/banners/banner-slate.svg) · [PNG](./brand/banners/banner-slate.png) |
| <img src="./brand/swatches/charcoal.svg" width="20" height="20" /> | <img src="./brand/icons/icon-charcoal.svg" width="28" height="28" /> | **Charcoal** | `charcoal` | `#27272a` | `rgb(39, 39, 42)` | [SVG](./brand/logos/logo-charcoal.svg) · [PNG](./brand/logos/logo-charcoal.png) | [SVG](./brand/icons/icon-charcoal.svg) · [PNG](./brand/icons/icon-charcoal.png) · [ICO](./brand/icons/icon-charcoal.ico) | [SVG](./brand/banners/banner-charcoal.svg) · [PNG](./brand/banners/banner-charcoal.png) |
| <img src="./brand/swatches/white.svg" width="20" height="20" /> | <img src="./brand/icons/icon-white.svg" width="28" height="28" /> | **White** | `white` | `#ffffff` | `rgb(255, 255, 255)` | [SVG](./brand/logos/logo-white.svg) · [PNG](./brand/logos/logo-white.png) | [SVG](./brand/icons/icon-white.svg) · [PNG](./brand/icons/icon-white.png) · [ICO](./brand/icons/icon-white.ico) | [SVG](./brand/banners/banner-white.svg) · [PNG](./brand/banners/banner-white.png) |
| <img src="./brand/swatches/black.svg" width="20" height="20" /> | <img src="./brand/icons/icon-black.svg" width="28" height="28" /> | **Black** | `black` | `#09090b` | `rgb(9, 9, 11)` | [SVG](./brand/logos/logo-black.svg) · [PNG](./brand/logos/logo-black.png) | [SVG](./brand/icons/icon-black.svg) · [PNG](./brand/icons/icon-black.png) · [ICO](./brand/icons/icon-black.ico) | [SVG](./brand/banners/banner-black.svg) · [PNG](./brand/banners/banner-black.png) |

---

## 🤖 Official Discord Applications Media Kit (`Virtue`, `YourApps`, `TDL`, `Zodiac` & `Metamorphosis`)

Official first-party Discord applications developed by **Xernerx Studios** carry their own distinct visual identity, color palette, production imagery, and monochrome beta/canary assets in [`./brand/applications/`](./brand/applications) (and hosted at `https://www.xernerx.com/applications/<app>/`).

| Icon | Application | Slogan | Official Primary Color | Production Assets | Beta / Canary Assets |
| :---: | :--- | :--- | :--- | :---: | :---: |
| <img src="./brand/applications/virtue/icon.png" width="44" height="44" alt="Virtue Icon" /> | **[Virtue](https://www.xernerx.com/applications/virtue)**<br /><sub>Global & Server Discord Leveling Bot (`1484880634844287138`)</sub> | *Track. Grow. Ascend.* | <img src="./brand/swatches/virtue-gold.svg" width="14" height="14" /> **Celestial Gold** (`#f59e0b`) | [Icon PNG](./brand/applications/virtue/icon.png) · [Icon ICO](./brand/applications/virtue/icon.ico) · [Banner PNG](./brand/applications/virtue/banner.png) | [Beta Icon PNG](./brand/applications/virtue/icon-beta.png) · [Beta Icon ICO](./brand/applications/virtue/icon-beta.ico) · [Beta Banner PNG](./brand/applications/virtue/banner-beta.png) |
| <img src="./brand/applications/yourapps/icon.png" width="44" height="44" alt="YourApps Icon" /> | **[YourApps](https://www.xernerx.com/applications)**<br /><sub>Discord-Native Forms & Applications Bot (`619328560141697036`)</sub> | *Discord Forms & Applications* | <img src="./brand/swatches/yourapps-orange.svg" width="14" height="14" /> **Paper Plane Orange** (`#f97316`) | [Icon PNG](./brand/applications/yourapps/icon.png) · [Icon ICO](./brand/applications/yourapps/icon.ico) · [Banner PNG](./brand/applications/yourapps/banner.png) | [Beta Icon PNG](./brand/applications/yourapps/icon-beta.png) · [Beta Icon ICO](./brand/applications/yourapps/icon-beta.ico) · [Beta Banner PNG](./brand/applications/yourapps/banner-beta.png) |
| <img src="./brand/applications/todo/icon.png" width="44" height="44" alt="To-Do List Bot Icon" /> | **[To-Do List Bot (TDL)](https://app.xernerx.com/bots/todo)**<br /><sub>Collaborative Discord Task Boards & Checklists (`782105629572464652`)</sub> | *Collaborative Discord Task Boards & Checklists* | <img src="./brand/swatches/todo-primary.svg" width="14" height="14" /> **TDL Leaf Green** (`#71cc2e`) | [Icon PNG](./brand/applications/todo/icon.png) · [Icon ICO](./brand/applications/todo/icon.ico) · [Banner PNG](./brand/applications/todo/banner.png) | [Beta Icon PNG](./brand/applications/todo/icon-beta.png) · [Beta Icon ICO](./brand/applications/todo/icon-beta.ico) · [Beta Banner PNG](./brand/applications/todo/banner-beta.png) |
| <img src="./brand/applications/zodiac/icon.png" width="44" height="44" alt="Zodiac Icon" /> | **[Zodiac](https://app.xernerx.com/bots/zodiac)**<br /><sub>Daily Horoscopes, Sign Profiles & Cosmic Compatibility (`950251264095162418`)</sub> | *Daily Horoscopes & Astrology* | <img src="./brand/swatches/zodiac-primary.svg" width="14" height="14" /> **Zodiac Bronze** (`#8b520f`) | [Icon PNG](./brand/applications/zodiac/icon.png) · [Icon ICO](./brand/applications/zodiac/icon.ico) · [Banner PNG](./brand/applications/zodiac/banner.png) | [Beta Icon PNG](./brand/applications/zodiac/icon-beta.png) · [Beta Icon ICO](./brand/applications/zodiac/icon-beta.ico) · [Beta Banner PNG](./brand/applications/zodiac/banner-beta.png) |
| <img src="./brand/applications/metamorphosis/icon.png" width="44" height="44" alt="Metamorphosis Icon" /> | **[Metamorphosis](https://app.xernerx.com/bots/metamorphosis)**<br /><sub>Dynamic Voice Channels & Community Automation (`881678826906730547`)</sub> | *Dynamic Voice & Community Automation* | <img src="./brand/swatches/metamorphosis-sky.svg" width="14" height="14" /> **Dialogue Sky Blue** (`#199fd9`) | [Icon PNG](./brand/applications/metamorphosis/icon.png) · [Icon ICO](./brand/applications/metamorphosis/icon.ico) · [Banner PNG](./brand/applications/metamorphosis/banner.png) | [Beta Icon PNG](./brand/applications/metamorphosis/icon-beta.png) · [Beta Icon ICO](./brand/applications/metamorphosis/icon-beta.ico) · [Beta Banner PNG](./brand/applications/metamorphosis/banner-beta.png) |

---

### 1. Virtue — Official Imagery & Color Palette

<p align="center">
  <img src="./brand/applications/virtue/banner.png" alt="Virtue Official Banner — Track. Grow. Ascend." width="100%" />
</p>

| Production Icon | Production Banner | Beta / Canary Icon | Beta / Canary Banner |
| :---: | :---: | :---: | :---: |
| <img src="./brand/applications/virtue/icon.png" alt="Virtue Icon" width="120" /> | <img src="./brand/applications/virtue/banner.png" alt="Virtue Banner" width="320" /> | <img src="./brand/applications/virtue/icon-beta.png" alt="Virtue Beta Icon" width="120" /> | <img src="./brand/applications/virtue/banner-beta.png" alt="Virtue Beta Banner" width="320" /> |

#### Virtue Color Tokens

| Swatch | Color Name | Xernerx Preset | Hex | RGB | Role in Virtue Identity |
| :---: | :--- | :--- | :--- | :--- | :--- |
| <img src="./brand/swatches/virtue-gold.svg" width="20" height="20" /> | **Celestial Gold** *(Primary)* | `gold` | `#f59e0b` | `rgb(245, 158, 11)` | Primary Halo ring, outer wing radiance, and default XP milestone highlight |
| <img src="./brand/swatches/virtue-champagne.svg" width="20" height="20" /> | **Warm Champagne** | `peach` | `#fdba74` | `rgb(253, 186, 116)` | Inner angelic feather glow and warm celestial particle accents |
| <img src="./brand/swatches/virtue-ivory.svg" width="20" height="20" /> | **Radiant Ivory** | `white` | `#fff7ed` | `rgb(255, 247, 237)` | Central diamond core, starlight flares, and `VIRTUE` display lettering |
| <img src="./brand/swatches/virtue-obsidian.svg" width="20" height="20" /> | **Obsidian Void** | `black` | `#18191d` | `rgb(24, 25, 29)` | Deep celestial dark canvas background |

---

### 2. YourApps — Official Imagery & Color Palette

<p align="center">
  <img src="./brand/applications/yourapps/banner.png" alt="YourApps Official Banner — Discord Forms & Applications" width="100%" />
</p>

| Production Icon | Production Banner | Beta / Canary Icon | Beta / Canary Banner |
| :---: | :---: | :---: | :---: |
| <img src="./brand/applications/yourapps/icon.png" alt="YourApps Icon" width="120" /> | <img src="./brand/applications/yourapps/banner.png" alt="YourApps Banner" width="320" /> | <img src="./brand/applications/yourapps/icon-beta.png" alt="YourApps Beta Icon" width="120" /> | <img src="./brand/applications/yourapps/banner-beta.png" alt="YourApps Beta Banner" width="320" /> |

#### YourApps Color Tokens

| Swatch | Color Name | Xernerx Preset | Hex | RGB | Role in YourApps Identity |
| :---: | :--- | :--- | :--- | :--- | :--- |
| <img src="./brand/swatches/yourapps-orange.svg" width="20" height="20" /> | **Paper Plane Orange** *(Primary)* | `orange` | `#f97316` | `rgb(249, 115, 22)` | Origami paper airplane emblem and primary call-to-action accent |
| <img src="./brand/swatches/yourapps-peach.svg" width="20" height="20" /> | **Sparkle Peach** | `peach` | `#fdba74` | `rgb(253, 186, 116)` | Flight trajectory swoop arc and 4-point star sparkles |
| <img src="./brand/swatches/yourapps-teal.svg" width="20" height="20" /> | **Ocean Teal** | `cyan` | `#1e5f74` | `rgb(30, 95, 116)` | Atmospheric teal-blue background gradient midtone |
| <img src="./brand/swatches/yourapps-navy.svg" width="20" height="20" /> | **Deep Navy Canvas** | `charcoal` | `#162238` | `rgb(22, 34, 56)` | Deep navy gradient base and bold illustration outline stroke |

---

### 3. To-Do List Bot (TDL) — Official Imagery & Color Palette

<p align="center">
  <img src="./brand/applications/todo/banner.png" alt="To-Do List Bot (TDL) Official Banner" width="100%" />
</p>

| Production Icon | Production Banner | Beta / Canary Icon | Beta / Canary Banner |
| :---: | :---: | :---: | :---: |
| <img src="./brand/applications/todo/icon.png" alt="To-Do List Bot Icon" width="120" /> | <img src="./brand/applications/todo/banner.png" alt="To-Do List Bot Banner" width="320" /> | <img src="./brand/applications/todo/icon-beta.png" alt="To-Do List Bot Beta Icon" width="120" /> | <img src="./brand/applications/todo/banner-beta.png" alt="To-Do List Bot Beta Banner" width="320" /> |

#### To-Do List Bot (TDL) Color Tokens

| Swatch | Color Name | Xernerx Preset | Hex | RGB | Role in TDL Identity |
| :---: | :--- | :--- | :--- | :--- | :--- |
| <img src="./brand/swatches/todo-primary.svg" width="20" height="20" /> | **TDL Leaf Green** *(Official Bot Color)* | `lime` | `#71cc2e` | `rgb(113, 204, 46)` | Official To-Do List Bot brand & Discord embed accent color |
| <img src="./brand/swatches/todo-coral.svg" width="20" height="20" /> | **Checkmark Coral** | `coral` | `#ff6363` | `rgb(255, 99, 99)` | Completed task checkmarks and active checklist item highlights |
| <img src="./brand/swatches/todo-gold.svg" width="20" height="20" /> | **Clipboard Gold** | `yellow` | `#f5b82e` | `rgb(245, 184, 46)` | Top clipboard clasp accent and priority task indicator |
| <img src="./brand/swatches/todo-mint.svg" width="20" height="20" /> | **Mint Sage Gradient** | `mint` | `#8de0a6` | `rgb(141, 224, 166)` | Lower-right fresh productivity gradient wash |
| <img src="./brand/swatches/todo-sky.svg" width="20" height="20" /> | **Sky Azure Gradient** | `sky` | `#4392c7` | `rgb(67, 146, 199)` | Upper-left sky gradient base |

---

### 4. Zodiac — Official Imagery & Color Palette

<p align="center">
  <img src="./brand/applications/zodiac/banner.png" alt="Zodiac Official Banner" width="100%" />
</p>

| Production Icon | Production Banner | Beta / Canary Icon | Beta / Canary Banner |
| :---: | :---: | :---: | :---: |
| <img src="./brand/applications/zodiac/icon.png" alt="Zodiac Icon" width="120" /> | <img src="./brand/applications/zodiac/banner.png" alt="Zodiac Banner" width="320" /> | <img src="./brand/applications/zodiac/icon-beta.png" alt="Zodiac Beta Icon" width="120" /> | <img src="./brand/applications/zodiac/banner-beta.png" alt="Zodiac Beta Banner" width="320" /> |

#### Zodiac Color Tokens

| Swatch | Color Name | Xernerx Preset | Hex | RGB | Role in Zodiac Identity |
| :---: | :--- | :--- | :--- | :--- | :--- |
| <img src="./brand/swatches/zodiac-primary.svg" width="20" height="20" /> | **Zodiac Bronze** *(Official Bot Color)* | `gold` | `#8b520f` | `rgb(139, 82, 15)` | Official Zodiac brand & Discord embed accent color |
| <img src="./brand/swatches/zodiac-amber.svg" width="20" height="20" /> | **Crescent Amber Gold** | `orange` | `#fbb040` | `rgb(251, 176, 64)` | Crescent moon and 4-point star emblem |
| <img src="./brand/swatches/zodiac-periwinkle.svg" width="20" height="20" /> | **Constellation Periwinkle** | `indigo` | `#6d78ad` | `rgb(109, 120, 173)` | Radial zodiac sign wheel glyphs |
| <img src="./brand/swatches/zodiac-midnight.svg" width="20" height="20" /> | **Midnight Cosmos Navy** | `cobalt` | `#00104a` | `rgb(0, 16, 74)` | Deep night sky canvas background |

---

### 5. Metamorphosis — Official Imagery & Color Palette

<p align="center">
  <img src="./brand/applications/metamorphosis/banner.png" alt="Metamorphosis Official Banner" width="100%" />
</p>

| Production Icon | Production Banner | Beta / Canary Icon | Beta / Canary Banner |
| :---: | :---: | :---: | :---: |
| <img src="./brand/applications/metamorphosis/icon.png" alt="Metamorphosis Icon" width="120" /> | <img src="./brand/applications/metamorphosis/banner.png" alt="Metamorphosis Banner" width="320" /> | <img src="./brand/applications/metamorphosis/icon-beta.png" alt="Metamorphosis Beta Icon" width="120" /> | <img src="./brand/applications/metamorphosis/banner-beta.png" alt="Metamorphosis Beta Banner" width="320" /> |

#### Metamorphosis Color Tokens

| Swatch | Color Name | Xernerx Preset | Hex | RGB | Role in Metamorphosis Identity |
| :---: | :--- | :--- | :--- | :--- | :--- |
| <img src="./brand/swatches/metamorphosis-sky.svg" width="20" height="20" /> | **Dialogue Sky Blue** *(Primary)* | `sky` | `#199fd9` | `rgb(25, 159, 217)` | Circular icon disc and primary brand accent |
| <img src="./brand/swatches/metamorphosis-white.svg" width="20" height="20" /> | **Crisp White** | `white` | `#ffffff` | `rgb(255, 255, 255)` | Foreground speech bubble and primary banner wordmark |
| <img src="./brand/swatches/metamorphosis-black.svg" width="20" height="20" /> | **Obsidian Black** | `black` | `#000000` | `rgb(0, 0, 0)` | Counter-speech bubble and banner canvas |

---

### 6. Additional & Legacy Service Brand Colors

| Swatch | Service / Project | Xernerx Preset | Hex | RGB | Role |
| :---: | :--- | :--- | :--- | :--- | :--- |
| <img src="./brand/swatches/roblox-utilities.svg" width="20" height="20" /> | **Roblox Utilities** | `white` | `#f5f3f1` | `rgb(245, 243, 241)` | Official Warm Alabaster brand & embed accent color for Roblox Utilities |

---

## 📦 Official SDK Package Media Kit (`@xernerx/*`)

Each open-source TypeScript SDK package in the Xernerx ecosystem has an assigned official Xernerx color, a 2–3 letter scope code, a circular package badge icon (`870×870`), and a bespoke architectural banner (`1600×440` @ 2x):

| Icon | Package | Scope | Assigned Color | Package Icon (`870×870`) | Package Banner (`1600×440`) |
| :---: | :--- | :---: | :--- | :---: | :---: |
| <img src="./brand/packages/icons/xernerx.svg" width="36" height="36" /> | **[`xernerx`](https://docs.xernerx.com/packages/xernerx)** | `XRX` | <img src="./brand/swatches/purple.svg" width="14" height="14" /> **Purple** (`#8b7cf6`) | [SVG](./brand/packages/icons/xernerx.svg) · [PNG](./brand/packages/icons/xernerx.png) · [ICO](./brand/packages/icons/xernerx.ico) | [SVG](./brand/packages/banners/xernerx.svg) · [PNG](./brand/packages/banners/xernerx.png) |
| <img src="./brand/packages/icons/framework.svg" width="36" height="36" /> | **[`@xernerx/framework`](https://docs.xernerx.com/packages/@xernerx/framework)** | `XF` | <img src="./brand/swatches/indigo.svg" width="14" height="14" /> **Indigo** (`#6366f1`) | [SVG](./brand/packages/icons/framework.svg) · [PNG](./brand/packages/icons/framework.png) · [ICO](./brand/packages/icons/framework.ico) | [SVG](./brand/packages/banners/framework.svg) · [PNG](./brand/packages/banners/framework.png) |
| <img src="./brand/packages/icons/commands.svg" width="36" height="36" /> | **[`@xernerx/commands`](https://docs.xernerx.com/packages/@xernerx/commands)** | `XC` | <img src="./brand/swatches/cyan.svg" width="14" height="14" /> **Cyan** (`#06b6d4`) | [SVG](./brand/packages/icons/commands.svg) · [PNG](./brand/packages/icons/commands.png) · [ICO](./brand/packages/icons/commands.ico) | [SVG](./brand/packages/banners/commands.svg) · [PNG](./brand/packages/banners/commands.png) |
| <img src="./brand/packages/icons/extension-builder.svg" width="36" height="36" /> | **[`@xernerx/extension-builder`](https://docs.xernerx.com/packages/@xernerx/extension-builder)** | `XE` | <img src="./brand/swatches/gold.svg" width="14" height="14" /> **Gold** (`#f59e0b`) | [SVG](./brand/packages/icons/extension-builder.svg) · [PNG](./brand/packages/icons/extension-builder.png) · [ICO](./brand/packages/icons/extension-builder.ico) | [SVG](./brand/packages/banners/extension-builder.svg) · [PNG](./brand/packages/banners/extension-builder.png) |
| <img src="./brand/packages/icons/hooks.svg" width="36" height="36" /> | **[`@xernerx/hooks`](https://docs.xernerx.com/packages/@xernerx/hooks)** | `XH` | <img src="./brand/swatches/emerald.svg" width="14" height="14" /> **Emerald** (`#10b981`) | [SVG](./brand/packages/icons/hooks.svg) · [PNG](./brand/packages/icons/hooks.png) · [ICO](./brand/packages/icons/hooks.ico) | [SVG](./brand/packages/banners/hooks.svg) · [PNG](./brand/packages/banners/hooks.png) |
| <img src="./brand/packages/icons/stats.svg" width="36" height="36" /> | **[`@xernerx/stats`](https://docs.xernerx.com/packages/@xernerx/stats)** | `XS` | <img src="./brand/swatches/pkg-stats.svg" width="14" height="14" /> **Coral** (`#f43f5e`) | [SVG](./brand/packages/icons/stats.svg) · [PNG](./brand/packages/icons/stats.png) · [ICO](./brand/packages/icons/stats.ico) | [SVG](./brand/packages/banners/stats.svg) · [PNG](./brand/packages/banners/stats.png) |
| <img src="./brand/packages/icons/terminal.svg" width="36" height="36" /> | **[`@xernerx/terminal`](https://docs.xernerx.com/packages/@xernerx/terminal)** | `XT` | <img src="./brand/swatches/magenta.svg" width="14" height="14" /> **Magenta** (`#d946ef`) | [SVG](./brand/packages/icons/terminal.svg) · [PNG](./brand/packages/icons/terminal.png) · [ICO](./brand/packages/icons/terminal.ico) | [SVG](./brand/packages/banners/terminal.svg) · [PNG](./brand/packages/banners/terminal.png) |
| <img src="./brand/packages/icons/websocket.svg" width="36" height="36" /> | **[`@xernerx/websocket`](https://docs.xernerx.com/packages/@xernerx/websocket)** | `XW` | <img src="./brand/swatches/blue.svg" width="14" height="14" /> **Blue** (`#3b82f6`) | [SVG](./brand/packages/icons/websocket.svg) · [PNG](./brand/packages/icons/websocket.png) · [ICO](./brand/packages/icons/websocket.ico) | [SVG](./brand/packages/banners/websocket.svg) · [PNG](./brand/packages/banners/websocket.png) |

### Visual Gallery — SDK Package Banners

| `xernerx` (`XRX` · Purple `#8b7cf6`) | `@xernerx/framework` (`XF` · Indigo `#6366f1`) |
| :---: | :---: |
| <img src="./brand/packages/banners/xernerx.svg" alt="xernerx banner" width="100%" /> | <img src="./brand/packages/banners/framework.svg" alt="@xernerx/framework banner" width="100%" /> |
| **`@xernerx/commands` (`XC` · Cyan `#06b6d4`)** | **`@xernerx/extension-builder` (`XE` · Gold `#f59e0b`)** |
| <img src="./brand/packages/banners/commands.svg" alt="@xernerx/commands banner" width="100%" /> | <img src="./brand/packages/banners/extension-builder.svg" alt="@xernerx/extension-builder banner" width="100%" /> |
| **`@xernerx/hooks` (`XH` · Emerald `#10b981`)** | **`@xernerx/stats` (`XS` · Coral `#f43f5e`)** |
| <img src="./brand/packages/banners/hooks.svg" alt="@xernerx/hooks banner" width="100%" /> | <img src="./brand/packages/banners/stats.svg" alt="@xernerx/stats banner" width="100%" /> |
| **`@xernerx/terminal` (`XT` · Magenta `#d946ef`)** | **`@xernerx/websocket` (`XW` · Blue `#3b82f6`)** |
| <img src="./brand/packages/banners/terminal.svg" alt="@xernerx/terminal banner" width="100%" /> | <img src="./brand/packages/banners/websocket.svg" alt="@xernerx/websocket banner" width="100%" /> |

---

## 📏 Brand Usage Guidelines

### ✅ Do's
- **Use Official Color Variants:** Always select from the 27 official Xernerx preset colors or use `logo-white` / `logo-black` when placing marks over busy photography.
- **Maintain Clear Space:** Keep at least **20%** of the mark's width/height as unobstructed padding around the Winged Crest or Wordmark Banner.
- **Use Vector SVGs on the Web:** Prefer `.svg` assets for web pages and Markdown documentation for instant load times and infinite scaling; use `.png` for OpenGraph/social meta tags and `.ico` for native Windows/desktop executables.
- **Pair Official Fonts:** Use **Fredoka** for display headings and UI labels, and **Cascadia Code** for code snippets, CLI commands, and scope badges.

### ❌ Don'ts
- **Do Not Distort or Stretch:** Never alter the aspect ratio (`1:1` for `logo` and `icon`, `2000:990` for `banner`, `40:11` for SDK package banners).
- **Do Not Recolor Arbitrarily:** Do not apply off-palette gradients, drop shadows, or unapproved neon outlines to the Winged Crest.
- **Do Not Imply Official Endorsement:** Community plugins, third-party extensions, and external Discord bots built with `@xernerx/framework` may state *"Built with @xernerx/framework"*, but must not present themselves as official **Xernerx Studios** products without written permission.

---

## ⚖️ Trademark & Licensing Notice

The **Xernerx**, **Xernerx Studios**, and **Xernerx Suite** names, the Winged Crest logo, product icons, and official visual assets in [`./brand/`](./brand) are trademarks and proprietary brand assets of **Xernerx Studios** governed by the **[Xernerx Studios Proprietary & SaaS License v1.0](https://xernerx.com/license)**. Press, community creators, and partner integrations may use these unmodified assets for truthful attribution and editorial reference in accordance with the guidelines above.
