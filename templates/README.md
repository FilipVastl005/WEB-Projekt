# Mateo — Community-Driven Climate & Weather Platform

**Author:** Filip Vastl  
**Course / Project:** WEB-Projekt  
**Technologies:** HTML5, Tailwind CSS v4, Vanilla CSS & Client-Side JavaScript (Zero Backend)

## Overview
A lightweight, modern web portfolio and technical landing page for **Mateo** (Community-Driven Climate & Weather Platform). The platform democratizes hyper-local meteorological data through low-power hardware, autonomous mesh networks, and a multi-tier Zero-Trust Quality Control pipeline.

## Features
- **Atmospheric Background Banner**: Uses the serene mountain mist palette (`src/img/banner1.jpg`) in the hero section and philosophy quote strip, styled via a separate CSS stylesheet.
- **Light & Minimal Aesthetic**: Clean whites, slate neutrals, and gentle teal/amber accents—uncluttered and focused on content legibility.
- **Three Hardware Topologies**:
  1. *Topology 1 (Urban Edge)*: ESP32-C6 standalone Wi-Fi 6 with Target Wake Time (TWT) deep sleep and isolated air quality sensor heaters.
  2. *Topology 2 (Suburban & Farms)*: Sub-GHz LoRa sensor node with indoor Home Deck hub (`http://homedeck.local`), Home Assistant MQTT, and offline microSD logging.
  3. *Topology 3 (Off-Grid Communities)*: P2P LoRa mesh with solar community kiosk captive Wi-Fi portal (`http://community.weather`) and delay-tolerant store-and-forward sync.
- **Interactive Zero-Trust QC Simulator**: Pure client-side interactive widget showing how incoming telemetry packets pass through physical boundary checks, temporal rate-of-change filters, and spatial IDW validation with real-time SQI score updates.
- **Sustainable Economic Model**: Clear comparison between free open-source core and enterprise high-frequency API access.
- **Accessible FAQ Accordion**: Built with native HTML `<details name="faq-group">` and `<summary>` elements.
- **Pure Client-Side Form**: Form submission runs entirely in browser JavaScript with `event.preventDefault()`—no backend, no database, no server required.

## File Organization
- [templates/index.html](file:///c:/Users/filip/Documents/WEB-Projekt/templates/index.html) — Main website file.
- [src/css/input.css](file:///c:/Users/filip/Documents/WEB-Projekt/src/css/input.css) — Source CSS importing Tailwind CSS and defining banner rules.
- [src/css/style.css](file:///c:/Users/filip/Documents/WEB-Projekt/src/css/style.css) — Compiled separate CSS stylesheet linked in the HTML.
- [src/img/banner1.jpg](file:///c:/Users/filip/Documents/WEB-Projekt/src/img/banner1.jpg) — Mountain banner background.

## Recompiling CSS
```bash
npm run build:css
```
Or for live watching during development:
```bash
npm run watch:css
```