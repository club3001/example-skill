---
name: antigravity-master
description: "Strukturiertes, zuverlässiges Agenten-Workflow nach dem B.L.A.S.T.-Protokoll (inspiriert von Google Antigravity). Nutzen bei komplexen Automatisierungen, Projekt-Setups oder wenn der Nutzer ein zuverlässiges, planbasiertes Vorgehen will."
type: workflow
lifecycle: active
---

# Antigravity Master — B.L.A.S.T. Protokoll

Zuverlässiges, planbasiertes Arbeiten für komplexe Aufgaben. Zuverlässigkeit vor Geschwindigkeit. Keine Annahmen bei der Logik.

## Protocol 0: Initialisierung (Pflicht)
Bevor irgendetwas gebaut wird:
1. Lege Planungsdateien an (oder nutze bestehende):
   - `task_plan.md` → Phasen, Ziele, Checklisten
   - `findings.md` → Recherche, Erkenntnisse, Einschränkungen
   - `progress.md` → Was erledigt wurde, Fehler, Tests
2. Definiere die Projekt-Verfassung (Schema + Regeln).
3. Stoppe, bis die Discovery-Fragen beantwortet und der Blueprint freigegeben ist.

## Phasen (B.L.A.S.T.)

### B – Blueprint (Vision & Logik)
Stelle diese 5 Fragen:
1. North Star: Was ist das eine gewünschte Ergebnis?
2. Integrationen: Welche externen Dienste? Sind Zugänge bereit?
3. Source of Truth: Wo liegen die Hauptdaten?
4. Delivery: Wie und wohin soll das Ergebnis geliefert werden?
5. Behavioral Rules: Wie soll das System sich verhalten? (Ton, Verbote, Einschränkungen)

Data-First: Definiere Input/Output-Schema, bevor Code geschrieben wird.

### L – Link (Verbindungen)
Prüfe APIs und Zugänge. Baue minimale Tests. Nicht weiter, wenn Verbindungen nicht funktionieren.

### A – Architect (3 Schichten)
- Architecture: SOPs / klare Abläufe dokumentieren
- Navigation: Entscheidungsschicht (ruft Tools in Reihenfolge auf)
- Tools: Kleine, testbare, deterministische Skripte

### S – Stylize (Verfeinerung)
Ausgabe formatieren, dem Nutzer zeigen, Feedback einholen.

### T – Trigger (Auslieferung)
Automatisierung aktivieren (Cron, Webhook etc.) und dokumentieren.

## Wichtige Regeln
- Zuverlässigkeit vor Geschwindigkeit
- Nie Geschäftslogik raten
- Bei Fehlern: Analysieren → Fixen → Testen → SOP aktualisieren (Self-Annealing)
- Schema und Regeln sind Gesetz

## Vorgehen
1. Protocol 0 starten und Discovery-Fragen stellen.
2. Blueprint freigeben lassen.
3. Phasen nacheinander abarbeiten.
4. Fortschritt in den Planungsdateien festhalten.
