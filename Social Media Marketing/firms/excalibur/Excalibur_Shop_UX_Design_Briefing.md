# 🧭 Excalibur – UX & Design Briefing (für Shopify-Entwicklung)

**Version:** v1.0  
**Erstellt von:** @Designer (Excalibur Agentur)  
**Datum:** YYYY-MM-DD  

---

## 1️⃣ Gesamtprinzip

> *„Excalibur ist keine Produktmarke, sondern eine Galerie für Präzision.“*  

Der Shop kommuniziert **technische Eleganz, Ruhe und Kontrolle**.  
Die UX soll nicht „verkaufen“, sondern *Vertrauen durch Präzision* erzeugen.  
Alle UI-Elemente sind funktional, ruhig und fein typografiert.  
Keine Animationen, die ablenken – Bewegung entsteht durch Licht, nicht durch Effekte.

---

## 2️⃣ Design-System Übersicht

| Kategorie | Spezifikation |
|------------|----------------|
| **Grundfarben** | `#0f0f0f` (Deep Black), `#1b1b1b` (Graphite), `#d4af37` (Gold Accent), `#f5f6f7` (Text White) |
| **Nischen-Akzente** | Yacht – Marineblau `#1a2a4f` · Jet – Titan-Silber `#c9cfd5` · Motorrad – Kupfer `#b87333` · Automobil – Burgund `#582f31` |
| **Typografie** | **Font Family:** Inter / Neue Montreal (Sans Serif) <br> **Weights:** 300 / 400 / 600  <br> **Base Size:** 16 px (1 rem) · H1: 56 px · H2: 32 px · Body: 18 px |
| **Spacing-System** | 8-Point Grid – Abstände in Vielfachen von 8 px (8, 16, 24, 32, 64 px) |
| **Iconografie** | Minimal, line-based, 1.5 px Stroke, Farbe `#f5f6f7` |
| **Buttons / CTAs** | Primär: Gold-Outline auf Graphit Hintergrund · Hover: gefüllt Gold mit Text in #0f0f0f |
| **Karten / Blöcke** | 12 px Radius, Shadow 0 2 12 rgba(255,255,255,0.05) |

---

## 3️⃣ Layout-Architektur (Shopify + Lovable)

### 🏠 **Startseite**

| Bereich | Element | Technische Umsetzung |
|----------|----------|----------------------|
| **Hero-Header** | Vollbreite `.webm` Video-Loop (5 s, muted) · Overlay Gradient (top→bottom #0f0f0f to transparent 60%) · Textblock zentriert | Lovable „Video Hero Section“ mit Custom Overlay Text |
| **Intro-Text** | 2–3 Sätze in H2-Format, max-width 720 px, mittig, viel Whitespace | Lovable Text Section |
| **Grid-Kollektionen** | 2×2 Layout, je Tile 1 Video-Loop + Overlay Text + CTA | Lovable Custom „Video Tile Grid“ Section |
| **Produkt-Highlight** | 1 großes Bild (Shopify Dynamic Product) + Text und „Jetzt entdecken“-CTA | Lovable Product Feature Section |
| **Philosophie** | Bild/Text-Kombination + Light-to-Dark-Gradient | Lovable Image/Text Block |
| **Newsletter / Footer** | Minimal Layout, 1 Zeile Text + Input + CTA | Lovable Footer Section |

---

### 🏍 **Produktseite (z. B. Motorrad – Mechanic Soul)**

| Bereich | Inhalt | Shopify Implementierung |
|----------|--------|-------------------------|
| **Hero-Video** | 6 s .webm Loop (keine Tonspur) | Lovable „Video Header“ mit Overlay Text |
| **Produkt-Infos** | Titel, Kurzbeschreibung, technische Stichpunkte | Standard Product Block + Custom Metafields |
| **Bundle-Auswahl** | 4 Optionen (Classic / Precision / Master / Cloths) | Shopify Bundles App oder Custom Variant Selector |
| **Anwendung** | Kurzer Text + Icon-Reihe (Material, Wirkung, Menge) | Custom Collapsible Block |
| **Trust / CTA** | „Add to Ritual“ Button, Gold-Akzent · Darunter Trust-Icons | Custom CTA Component |

---

### 🧩 **Philosophie / Pflegewissen**

- Standard-Pages mit Bild/Text-Blöcken  
- Typo großzügig gesetzt, Zeilenabstand 1.8  
- Abbildungen mit Schattierung und Negativraum  

---

## 4️⃣ Bild / Video Spezifikationen

| Asset | Format | Größe | Hinweise |
|--------|---------|--------|----------|
| **Hero-Videos (4 Nischen)** | `.webm` (autoplay, loop, muted) | ≤ 8 MB · 6–8 s | Einheitlicher Kamerawinkel und Licht Setting |
| **Produktbilder / Packshots** | `.jpg` oder `.webp` | 1200 × 1200 px | Realistische Flasche, sichtbares Label, kontrolliertes Licht |
| **Backgrounds** | `.png` | 1920 × 1080 px | Dunkle Textur, Gradient Graphit→Schwarz |

---

## 5️⃣ UX Richtlinien

| Prinzip | Beschreibung |
|----------|---------------|
| **Kognitive Ruhe** | Max. 3 visuelle Ebenen pro Viewport (Background / Content / CTA) |
| **Leserhythmus** | Überschriften → kurze Absätze → Bullet Infos |
| **Scrollverhalten** | sanft, kein Parallax, kein Autoplay Audio |
| **Hover Feedback** | Nur Lichtverlauf oder Farbänderung des Rahmens, keine Bewegung |
| **Mobile Priorität** | 1-Spalten Layout · Videos auf < 600 px durch Poster Image ersetzen |

---

## 6️⃣ Interaktion & Bewegung

- **Videos:** nur autoplay + loop, nie on-scroll-triggered  
- **Transitions:** `opacity` / `filter blur(8px)` – Dauer 250 ms  
- **CTA Hover:** `transition: all 0.3s ease; background-color:#d4af37; color:#0f0f0f;`  
- **Bundle-Selector:** sanfte Fade-Transition beim Variantwechsel  
- **Newsletter CTA:** Micro-interaction → Gold Line aufleuchten beim Focus  

---

## 7️⃣ Accessibility & Usability

- Kontrast > 7:1 zwischen Text und Background  
- Focus States sichtbar (Gold Outline)  
- ARIA Labels für alle CTAs  
- Video Poster Images für Screenreader  
- Touch-Flächen ≥ 44 × 44 px  

---

## 8️⃣ Dateistruktur / Naming

```
/assets
  /videos
    excalibur-yacht-hero.webm
    excalibur-jet-hero.webm
    excalibur-motorcycle-hero.webm
    excalibur-automotive-hero.webm
  /images/products
    excalibur-yacht-cleaner-classic.jpg
    excalibur-motorcycle-cleaner-master.jpg
  /images/backgrounds
    graphite-gradient.png
```

---

## 9️⃣ Deliverables für Entwicklung

| Datei / Format | Zweck |
|-----------------|-------|
| `/design-system.json` | Farb- & Typo-Tokens für Theme Customizer |
| `/ux-guide.md` | Dieses Briefing (Referenz für Dev Team) |
| `/assets/videos/*.webm` | Hero-Loops (4 Nischen) |
| `/assets/images/products/*.jpg` | KI-optimierte Packshots |
| `/brand-palette.png` | Visual Reference für Akzentfarben |
| `/typography-spec.png` | Beispiel Textgrößen / Abstände |

---

## 10️⃣ Qualitäts-Checkliste vor Go-Live

- [ ] Kontrast zwischen Text und Hintergrund ≥ 7:1  
- [ ] Alle Hero-Videos laden ≤ 2 s  
- [ ] Responsive Breakpoints getestet (≥ 360 px → 4K)  
- [ ] Labels auf Flaschen lesbar (keine Überbelichtung)  
- [ ] Bundle-Selector funktioniert fehlerfrei  
- [ ] CTA-Hover ruhig und responsiv  

---

**→ Ziel:**  
Ein Excalibur-Shop, der sich **wie eine präzise gefertigte Maschine** verhält:  
ruhig, elegant, technisch perfekt.
