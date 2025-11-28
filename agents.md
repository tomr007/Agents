# Agents (Router)

Diese Datei ist der zentrale Einstiegspunkt für alle Agentenanfragen. Jede Anfrage wird anhand des beschriebenen Themas automatisch an das passende Team weitergeleitet – auch wenn kein spezifischer Agent genannt wird.

## Routing-Entscheidung
1. **Sales / Vertrieb** – Begriffe wie „Lead“, „Deal“, „Opportunity“, „Pipeline“, „CRM“, „Vertrieb“, „Sales“, „Account“. → Weiterleitung an das Sales-Team (siehe `Sales-Team/sales-agents.md`).
2. **Marketing / Content** – Begriffe wie „LinkedIn“, „Content“, „Social Media“, „SEO“, „Ads“, „Design“, „Kampagne“. → Weiterleitung an das Social-Media-/Marketing-Team (siehe `Social Media Marketing/marketing-agents.md`).
3. **Unklarer Kontext** – Falls weder Sales noch Marketing eindeutig erkennbar sind, wird eine kurze Rückfrage zum gewünschten Ziel gestellt und danach weitergeleitet.

## Standardverhalten ohne Agentennennung
- **Sales-Anfragen**: Starte mit dem Sales-**coordinator** für CRM- und Pipeline-Updates. Falls Messaging, Coaching oder Gesprächsleitfäden benötigt werden, schaltet der Router den **coach** hinzu.
- **Marketing-Anfragen**: Starte mit dem **strategist**, der den passenden Spezialisten (SEO-Planner, SM-Planner, Designer, Writer, Videographer, Chief Editor, Publisher oder Workflow-Koordinator) auswählt.

## Erweiterbarkeit
- Neue Teams lassen sich ergänzen, indem hier ein Routing-Stichpunkt ergänzt und eine passende `*-agents.md` Datei angelegt wird.
- Existierende Teams können weitere Rollen hinzufügen, solange ihre Teamdatei den Einstieg und Default-Agent definiert.
