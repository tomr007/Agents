# CRM Schema
- YAML-Header enthält: `id`, `version`, `account`, `stage`, `status`, `created`, `updated`, `source`, `campaign`, `company`, `contact`, `value`, `owner`, `next_step`, `history`, `analysis`, `notes`.
- `account` ist Pflicht zur Mandantentrennung.
- `history` als Liste im Blockstring-Format, jede Änderung mit Datum.
- `notes` als Liste mit Datum, Autor, Inhalt.
