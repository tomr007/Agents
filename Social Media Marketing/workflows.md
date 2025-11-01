# 🧭 Content Workflow – Agentenrichtlinien

Dieses Repository definiert alle Agentenrollen, ihre Übergaben und Regeln für die KI-gestützte Content-Erstellung.  
Die Architektur folgt dem Prinzip: **Mensch orchestriert – KI assistiert.**

---

## 🎯 Ziel
Effiziente Erstellung und Planung von Inhalten (Texte, Bilder, Posts) auf Basis strategisch definierter Personas, Themen und Nischen.

---

## 🧩 Grundprinzipien
1. **Jeder Agent arbeitet auf Basis freigegebener Informationen.**
   - Konsultiere das kundenspezifische Readme (z. B. `firms/<slug>/readme.md`) und kläre, welche Briefings und Dokumente für den aktuellen Fall herangezogen werden sollen.
   - Stelle sicher, dass alle Rollen das zentrale Firmen-Readme unter `https://github.com/tomr007/Agents/blob/main/Social%20Media%20Marketing/firms/<firm-slur>/readme.md` als Startpunkt für Kontexte und Briefings nutzen. Besteht Unsicherheit über den korrekten `<firm-slur>`, wird dieser zuerst mit dem Nutzer geklärt.
2. **Der Mensch ist der Orchestrator.**
   KI-Agenten liefern Vorschläge, keine finalen Entscheidungen.
3. **Alle Ergebnisse sind versionierbar und transparent.**
4. **Datenflüsse sind sequenziell, aber flexibel:**  
   Stratege → Chefredakteur → Texter → Designer → Planer → Publisher
5. **Feedbackschleifen sind erlaubt.**  
   Der Nutzer kann jeden Agenten erneut aufrufen, um Korrekturen oder Vertiefungen vorzunehmen.

---

## 💬 Standard-Interaktion
- Jeder Agent wird im Chat über `@AgentName` angesprochen.  
- Jeder Agent versteht folgende Befehle:
  - `@AgentName init` → startet neuen Workflow-Schritt
  - `@AgentName refine` → verbessert vorherige Ausgabe
  - `@AgentName handoff @NextAgent` → übergibt die Ergebnisse an nächsten Agenten

---

## 🗃️ Datenstrukturen (Beispiele)

| Kategorie | Beispielinhalt | Gespeichert als |
|------------|----------------|----------------|
| Readme | Index, Dokumentenstand | `firms/<slug>/readme.md` |
| Firma | Stammdaten, Markenplattform | `firms/<slug>/00_company-profile.md` |
| Produkte/Services | Nutzen, Proof-Points | `firms/<slug>/product-<slug>.md` bzw. `firms/<slug>/service-<slug>.md` |
| Nische | Angebots-Zuordnung, Marktdynamik | `firms/<slug>/niche-<slug>.md` |
| Persona | Profil, Needs, Kanal-Keywords | `firms/<slug>/persona-<slug>.md` |
| Thema | Titel, Keywords, Beschreibung | `topics/NAME.md` |
| Content-Idee | Headline, Kurztext, Zielgruppe | `ideas/ID.md` |
| Bild | Prompt, Stil, Canva-Link | `visuals/ID.md` |
| Planung | Kanal, Datum, Status | `plan/ID.md` |

---

## 🔗 Empfohlene Tools
- **ChatGPT Projects / Claude Workspaces** für die Interaktion  
- **GitHub** zur Versionierung der Agenten und Ergebnisse  
- **Canva** für visuelle Umsetzung  
- **ClickUp / Supabase** zur Verwaltung von Content-Backlogs und Zeitplänen  

---

## ⚙️ Beispielablauf

1. `@Strategist` entwickelt Persona und Themencluster
2. `@ChiefEditor` legt redaktionelle Leitlinien fest  
3. `@Writer` erstellt Content-Exposés und Headlines  
4. `@Designer` erzeugt KI-Bilder und Canva-Layouts  
5. `@Planner` plant Veröffentlichungszeitpunkte  
6. `@Publisher` veröffentlicht und archiviert Ergebnisse

---

**Letzte Regel:**  
> KI unterstützt, aber du entscheidest.  
> Nur Inhalte, die du manuell freigibst, gelten als veröffentlicht.

### Datenablage
- [`workflows/runbook.md`](workflows/runbook.md): Halte Koordinationsprozesse, Kommunikationsroutinen und Eskalationspfade detailliert fest.
- [`workflows/coordination-board.json`](workflows/coordination-board.json): Pflege den strukturierten Überblick über Kampagnenstatus je Rolle und nächste Abstimmungen.

> Hinweis: Aktualisiere Runbook und Board nach jedem Team-Sync und verlinke bei Anpassungen die relevanten Agenten-Dokumente für Transparenz.

