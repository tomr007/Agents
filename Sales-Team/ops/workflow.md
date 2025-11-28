# Workflow
1. Nutzer liefert Freitext-Update oder neuen Lead.
2. Agent extrahiert strukturierte Daten und Mandant (`account`).
3. CRM-Dokument öffnen/erstellen, YAML aktualisieren (`updated`, `history`, `notes`).
4. `coordinator` prüft Pipeline-Stufe und Next Step, `coach` liefert Messaging/Playbook-Hinweise.
5. Rückmeldung an Nutzer mit Zusammenfassung und empfohlenen Aktionen.
