# 🎨 Excalibur – Designer Asset Production Table

**Projekt:** Excalibur Luxury Surface Care Boutique  
**Agent:** @Designer  
**System:** Shopify + Lovable Theme  
**Version:** v1.0 (Launch-Setup mit 4 Nischen)

---

| ID | Seite | Asset | Position im Shop | Prompt-Briefing (inkl. Keywords) | Format / Output |
|----|--------|--------|------------------|----------------------------------|-----------------|
| **A-004** | `/` | 4 Grid-Tiles | Startseite → Hauptnavigation | *Erzeuge ein symmetrisches 2×2 Grid mit dunklem Hintergrund (`#0f0f0f→#1b1b1b`). Jede Kachel repräsentiert eine Nische (Motorrad, Auto, Yacht, Flugzeug) mit ruhigem Lichtverlauf und Overlay-Text. Keywords: Reinheit, Präzision, Oberfläche, Klarheit.* | `.json` / Shopify Section |
| **A-010** | `/` | Hintergrundverlauf | Global → Seitenhintergrund | *Erstelle einen dezenten dunklen Gradient-Hintergrund `#0f0f0f→#1b1b1b` mit weichem Licht von oben. Keywords: Oberfläche, Struktur, Tiefe.* | `.png` (1920×1080) |
| **A-012** | `/collections` | Grid mit 4 Welten | Kollektionenübersicht | *Erzeuge eine 4-Tile-Galerie mit gleichmäßigem Abstand, identischem Seitenverhältnis, und Overlay-Farben pro Nische: Anthrazit (Motorrad), Burgund (Auto), Marine (Yacht), Eisweiß (Jet). Keywords: Präzision, Materialästhetik.* | `.json` / `.png` |
| **A-015** | `/collections/motorcycle` | KI-Packshot | Produktseite Hero | *Fotorealistische schwarze 0,5 l Sprühflasche mit dunklem Label. Licht: von links oben, Hintergrund: gebürsteter Stahl. Keywords: Mechanik, Oberfläche, Präzision, Reinheit.* | `.jpg` (1200×1200) |
| **A-016** | `/collections/motorcycle` | Bundle-Fotos (4 Varianten) | Produktgrid | *Erstelle Flat-Lay-Darstellungen der Flasche mit Mikrofasertüchern auf metallischem Untergrund. Varianten: Classic / Precision / Master / Cloths. Keywords: Pflege, Kontrolle, Material, Struktur.* | `.jpg` |
| **A-019** | `/collections/automotive` | KI-Packshot | Produktseite Hero | *Fotorealistische schwarze 0,5 l Sprühflasche mit Burgund-Gold-Reflex. Hintergrund: glänzende Karosseriefläche. Keywords: Glanz, Oberfläche, Linie, Präzision.* | `.jpg` |
| **A-020** | `/collections/automotive` | Bundle-Fotos | Produktgrid | *Flat-Lay Setup mit Leder, Glas und Chromreflexen; Kombination aus Flasche und Tuch. Keywords: Oberfläche, Detail, Pflege, Beständigkeit.* | `.jpg` |
| **A-023** | `/collections/yacht` | KI-Packshot | Produktseite Hero | *Schwarze Flasche, Reflex in Marineblau und Silber, Untergrund Edelstahl oder Gelcoat. Keywords: Salz, Sonne, Glanz, Oberfläche, Beständigkeit.* | `.jpg` |
| **A-024** | `/collections/yacht` | Bundle-Fotos | Produktgrid | *Set-Darstellung auf Bootskontext (Teakholz oder Chrom), mit Mikrofasertuch. Keywords: Reinheit, Oberfläche, Wasser, Beständigkeit.* | `.jpg` |
| **A-027** | `/collections/jet` | KI-Packshot | Produktseite Hero | *Schwarze Flasche, Lichtreflex in Eisweiß & Titan-Silber; Hintergrund: Hangar-Aluminium. Keywords: Transparenz, Aerodynamik, Reinheit, Präzision.* | `.jpg` |
| **A-028** | `/collections/jet` | Bundle-Fotos | Produktgrid | *Flat-Lay mit Aluminiumstruktur und antistatischem Look. Kombination aus Flasche, Tuch und Glasdetail. Keywords: Oberfläche, Klarheit, Technologie.* | `.jpg` |
| **A-033** | `/cart` | Cart-Layout | Warenkorb | *Erstelle minimalistisches Cart-Design mit schwarzem Hintergrund, goldener Fortschrittsanzeige (`#d4af37`) und weißer Typo. Keywords: Klarheit, Kontrolle, Ruhe.* | `.json` / `.liquid` |
| **A-034** | `/checkout` | Checkout-Flow | Checkout-Seite | *Gestalte linearen Checkout mit Progress-Bar in Gold, klarer Typografie, Weißraum. Keywords: Kontrolle, Präzision, Ruhe.* | `.json` / `.liquid` |
| **A-036** | `/newsletter` | CTA-Banner | Footer / Newsletter | *Minimaler Banner auf dunklem Grund, subtile Lichtkante, CTA „Erhalte Zugang zu limitierten Editionen“. Keywords: Exklusivität, Vertrauen, Klarheit.* | `.json` / `.png` |
| **A-038** | Global | Brandpalette | Designsystem | *Erstelle Tailwind-kompatible Farb- und Typo-Systemdatei mit HEX-Codes, Gradient-Definitionen und Font-Stack. Keywords: Präzision, Konsistenz.* | `.json` / `.md` |
| **A-041** | Global | Favicon / Logo | Browser + Header | *Erzeuge Excalibur-Schriftzug (Serif-Sans-Mix) in Gold auf Schwarz (#d4af37 / #0f0f0f). Varianten: 32 px, 64 px, SVG-Version. Keywords: Präzision, Luxus, Understatement.* | `.svg` / `.png` |

---

## 🔑 Hinweise zur Integration

- **Naming Convention:** `excalibur-[niche]-[assettype].[ext]`  
  *Beispiel:* `excalibur-motorcycle-packshot.jpg`  

- **Alt-Text / SEO:**  
  Verwende strukturierte Beschreibung:  
  *„Excalibur Oberflächenpflege für [Nische] – Reinheit, Präzision, Glanz.“*  

- **Color Consistency:**  
  - Motorrad → Anthrazit + Kupferlicht  
  - Auto → Burgund + Champagner-Gold  
  - Yacht → Marine + Silber  
  - Jet → Eisweiß + Titan-Silber  

---

*Stand: {{heutiges Datum einsetzen}}*
