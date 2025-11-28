# Sales-Team: Mandantenfähiges CRM- und Agenten-System

Dieses Verzeichnis bildet ein vollständig dateibasiertes, mandantenfähiges CRM für das Vertriebsteam ab. Alle Inhalte sind so strukturiert, dass KI-Agenten sie unmittelbar nutzen können.

## Ziele
- Leads aufnehmen, strukturieren und im YAML-Format pflegen.
- Zwei Agentenrollen: **coordinator** (Pipeline, Forecast, Controlling) und **coach** (Sales-Beratung, Next Steps, Psychologie, Messaging).
- Mandantenfähigkeit durch Accounts und ein wiederverwendbares Company-Template.
- Globale und mandantenspezifische Playbooks, Skripte und Voice-Guides.

## Struktur
- `agents/`: Agentenbeschreibungen für Routing und Aufgaben.
- `crm/`: Ein-Dokument-CRM mit Template und Beispieldaten.
- `accounts/`: Mandantenspezifische Assets (Playbooks, Skripte, Voice, Account-Metadaten).
- `company-template/`: White-Label-Vorlage für neue Mandanten.
- `global-playbooks/` & `global-scripts/`: Teamweite Standards als Fallback.
- `reviews/`: Templates für Opportunity- und Deal-Reviews.
- `ops/`: Pipeline-Definition, CRM-Schema, Workflow und Glossar.

## Arbeitsprinzipien
1. Jede Opportunity lebt in einem einzigen Markdown-Dokument mit YAML-Header.
2. Änderungen erfolgen durch Update des YAML-Blocks und Anhängen in `history` und `notes`.
3. Mandantenkontext wird im Feld `account` festgehalten; ohne Kontext wird nachgefragt.
4. Globale Inhalte dienen als Fallback, können aber je Account überschrieben werden.
