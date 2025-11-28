# Agent Router (Top-Level)

Dieser Router-Agent steuert alle eingehenden Anfragen und entscheidet anhand der Nutzerabsicht, welches Team zuständig ist.

## Routing-Logik
1. Begriffe wie „Lead“, „Deal“, „Opportunity“, „Vertrieb“, „Sales“ oder „Account“ → Sales-Team (/Agents/Sales-Team/agents).
2. Begriffe wie „LinkedIn Post“, „Content“, „Social Media“, „SEO“ oder „Design“ → Social-Media-/Marketing-Team (/Agents/Social Media Marketing/agents).
3. Falls der Kontext unklar ist, wird nach dem gewünschten Team gefragt und anschließend weitergeleitet.

## Ziel
- Neutrale, top-level Steuerung über alle Teams hinweg.
- Erweiterbar, falls neue Teams wie Customer Success oder Support hinzukommen.
