# Coiled Soul Studio — Site Redesign Notes

**Date:** 2026-06-20
**Goal:** Make the site look distinctive and crafted, not like a generic AI-generated template, while staying true to the Rooted Soul brand spirit (warm, handmade, refined, intentional).

This pass implemented four of a larger set of recommendations. Items 5 (process/making photos), 6 (commission / available-work on Connect), and 7 (scroll animation) were intentionally deferred.

## What changed and why

### 1. Hero — one line + one image instead of a paragraph
The home page used to open with the full maker bio set in italic serif. It now opens with a display headline ("Living sculptures with a *soul*") plus a single supporting line and a "View the work" button, paired with one hero image. The full bio moved below into a proper story section. **Why:** a template opens with a wall of text; a designed site leads with a clear statement and lets the work carry the page.

### 2. New type system (deviation from current brand guide — see below)
- **Display / headlines:** Cormorant Garamond → **Fraunces** (a crafted, high-contrast humanist serif with optical sizing). Reads as editorial and made-by-hand rather than the default "elegant serif" every AI site uses.
- **Body / UI:** DM Sans → **Hanken Grotesk** (a warmer humanist sans).
- Body copy is now **upright**, not italic. Italic is reserved for emphasis, taglines, captions, and pull phrases — the way it's meant to be used.

### 3. Palette shifted to the brand's "Kiln & Terroir" option
Adopted Palette Option 2 from the brand guide instead of the default earthy set:
- Replaced the old terracotta `#8B4513` (which is literally the CSS named color "SaddleBrown" — a giveaway) with **Rich Terracotta `#B05C52`**.
- Added **Oxblood `#7B2D2D`** ("Maker's Mark") as the single signature accent — used for links, the active nav state, the CTA button, and the stamp divider.
- **Sage Moss `#6B7F5E`** and **Peach `#FFBE98`** available as supporting tones.
- This keeps the site fully on-brand while breaking the instantly-recognizable "AI terracotta" palette.

### 4. Craft texture + asymmetry
- A subtle fired-clay **grain overlay** sits over the whole page (low-opacity SVG noise, multiply blend).
- The plain 40px / 1px divider line was replaced with a small **ceramic-stamp motif** (a dashed ring + center dot in oxblood), echoing a maker's stamp pressed into clay.
- Layout is **asymmetric**: the home hero is an offset two-column grid (copy + image) with a small "Hand-built · one of a kind" badge overlapping the image, instead of everything centered.
- The story's first paragraph has a **drop cap** in Fraunces — a deliberate, hand-set editorial touch.
- The top bar now places the **logo left, nav right** (a real masthead) rather than the centered logo-over-centered-nav stack.

## ⚠️ Deviation from the official Brand Guide

The brand guide (v1.0, April 2026) specifies **Cormorant Garamond + DM Sans** as the type system and the original primary palette. This redesign **deliberately changes the fonts** to make the site distinctive, and **promotes the brand's own alternate "Kiln & Terroir" palette** to primary on the web.

The palette change is within the brand guide (it's Option 2). The **font change is a genuine deviation.** It does not violate any brand *don't* (Fraunces and Hanken Grotesk are refined, not script/handwritten/decorative). 

**Action needed:** decide whether to (a) update the Brand Guide to make Fraunces + Hanken Grotesk the official system, or (b) revert the site to Cormorant + DM Sans. Recommendation: update the guide — the new pairing better serves the "crafted, not templated" goal the guide itself sets for the logo.

## Files touched
- `style.css` — full restyle (tokens, type, grain, stamp divider, hero, masthead).
- `index.html` — rebuilt hero + story + series preview.
- `series.html`, `connect.html`, `morning-routine.html`, `good-intentions.html`, `blue-heron.html`, `dear-friend.html` — new font links + new masthead header.

Image files, links, and page structure were left intact; all image paths verified.

## Deferred (not yet built)
- **5 — Process / "making" photos** (coils, wet clay, hands at work). A `Photos - website/Process/` folder already exists with "Jeans" in-progress shots ready to use when you are.
- **6 — Connect → commission / available work.** Connect is unchanged for now.
- **7 — Scroll/reveal animation.** Skipped by choice.
