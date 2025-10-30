# Strategist Firmen-Arbeitsräume

Jeder Workflow des Strategen wird als Firmenarbeitsraum in diesem Ordner abgelegt. Verwende **konsistente Slugs** (z.\u202fB. `acme-industries`) für die Verzeichnisnamen.

## Struktur einer Firma

```
firms/<firm-slug>/
├── 00_company-profile.md      # Basisdaten zur Firma, Vision, Kontaktpersonen
├── 01_brand-platform.md       # Markenwerte, USP-Übersicht, Tone of Voice
├── products/                  # Einzelne Produkte mit Nutzen und Proof
│   └── <product-slug>.md
├── services/                  # Dienstleistungen analog zu Produkten
│   └── <service-slug>.md
├── niches/                    # Markt- bzw. Themen-Nischen
│   └── <niche-slug>/
│       ├── _index.md          # Nischenbeschreibung, adressierte Angebote
│       └── personas/
│           └── <persona-slug>.md
└── research-log.md            # Quellen, Markt-Insights, offene Validierungen
```

## Persona-Dateien
Jede Persona-Datei folgt der Struktur:

```
# Persona: <Name>

## Profil
- **Rolle / Kontext:**
- **Entscheidungskompetenz:**
- **Reifegrad & Trigger:**

## Needs & Jobs-to-be-done
- Pain-Reliever (welche Angebote lösen welches Problem?)
- Gain-Creator (welchen Mehrwert erwartet die Persona?)

## Channel-Keywords
| Kanal | Such-/Trigger-Keywords | Content-Formate |
|-------|------------------------|-----------------|
| SEO   |                        |                 |
| Social|                        |                 |
| Ads   |                        |                 |
| Email |                        |                 |

## Messaging-Hinweise
- Tonalität / Stil
- Proof-Points
- Call-to-Action Hinweise
```

## Arbeitsweise
1. **Bestehenden Kunden aufrufen:** Nutze `@strategist init` und frage zuerst, ob für eine vorhandene Firma weitergearbeitet werden soll. Liste aktive Firmen-Slugs aus diesem Ordner auf.
2. **Neue Kampagne anlegen:** Wenn eine neue Firma oder Kampagne gestartet wird, lege die oben beschriebene Ordnerstruktur an und befülle die Startdokumente.
3. **Synchronisation:** Pflege Querverweise zu `strategist/datenlog.md` und `strategist/persona-index.json` (z.\u202fB. Persona-ID, letzter Stand, offene Fragen).

### Templates nutzen
- Unter [`strategist/firms/templates/`](templates/) findest du Markdown-Vorlagen für Firmenprofile, Markenplattform, Produkte, Services, Nischen, Personas und Research-Logs.
- Kopiere die gewünschten Dateien in den neuen Firmenordner und entferne das Suffix `.template` bei der Verwendung.

> Hinweise:
> - Lege nur die Ordner an, die benötigt werden (z.\u202fB. `products/` oder `services/`).
> - Verwende ISO-Datumsformate (`YYYY-MM-DD`) für Zeitstempel in den Dateien.
> - Verknüpfe Nischen und Personas klar mit den Produkten/Services, um Übergaben an Planner und Writer zu erleichtern.
