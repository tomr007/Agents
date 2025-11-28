# CRM (Ein-Dokument-Ansatz)

Jeder Lead, jede Opportunity und jeder Deal wird in einer einzelnen Markdown-Datei mit YAML-Header gepflegt. Änderungen erfolgen direkt im YAML und in fortlaufenden Abschnitten für History und Notizen.

## Prinzipien
- Keine Dubletten: pro Vorgang genau ein Dokument.
- Mandantenzuordnung über den `account`-Block im YAML.
- `updated`-Feld und `history` werden bei jeder Änderung ergänzt.
- Globale und Account-Playbooks stehen als Referenz bereit.

## Dateien
- `records/lead-template.md`: Vorlage mit allen benötigten Feldern inkl. Mandant.
- `records/example-lead-2025-001.md`: Beispiel, das den Mandantenkontext demonstriert.
