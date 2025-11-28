---
id: LD-2025-XXX
version: 1.0

# Mandant / Auftraggeber
account:
  id: AC-XXXX
  name: "LeanDigital GmbH"
  path: "../../accounts/LeanDigital"

# Pipeline
stage: lead          # lead | qualified | opportunity | deal-won | deal-lost
status: active       # active | stalled | closed
created: YYYY-MM-DD
updated: YYYY-MM-DD

# Herkunft
source: LinkedIn     # LinkedIn | Empfehlung | Event | Inbound | Outbound
campaign: null

# Unternehmen
company:
  name:
  size:
  industry:
  website:

# Kontaktperson
contact:
  name:
  role:
  email:
  phone:

# Wert / Einschätzung
value:
  estimate: null     # mögliche Dealgröße
  probability: null  # Schätzung bei Opportunity

# Verantwortlicher
owner: rep

# Nächster Schritt
next_step:
  date:
  description:
  owner:

# Entwicklungsprotokoll (jede Änderung hier anhängen)
history: |
  - YYYY-MM-DD: Lead angelegt.

# Analyse & Insights
analysis:
  need: null
  pain: null
  urgency: null
  budget: null
  authority: null
  timeline: null

# Notizen (fortlaufend)
notes:
  - date: YYYY-MM-DD
    author: user
    content: "Erste Notiz eintragen"
  -
---
