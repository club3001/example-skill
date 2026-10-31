---
name: grok2api-explainer
description: "Erklärt das Projekt chenyme/grok2api einfach. Nutzen wenn der Nutzer nach grok2api, Grok API Gateway, Multi-Account Grok oder dem Repo fragt."
type: knowledge
lifecycle: active
---

# grok2api — Einfache Erklärung

**Repository:** https://github.com/chenyme/grok2api

Das ist ein **Community-Projekt** (kein offizielles xAI-Produkt). Es ist ein Multi-Account-API-Gateway für Grok Build, Grok Web und Grok Console.

## Was es macht
- Verwaltet mehrere Grok-Accounts in Pools
- Bietet einheitliche OpenAI- und Anthropic-kompatible Schnittstellen
- Unterstützt Chat, Bilder, Videos, TTS usw.
- Hat ein eingebautes Admin-Dashboard
- Ermöglicht Routing, Failover, Quota-Management und Proxy-Einstellungen

## Wichtige Punkte
| Punkt | Bedeutung |
|-------|----------|
| Multi-Account | Mehrere Accounts parallel nutzen |
| OpenAI-kompatibel | Funktioniert mit vielen bestehenden Tools/SDKs |
| Admin-Console | Web-Oberfläche zum Verwalten |
| Community | Nicht von xAI offiziell unterstützt |

## Schnellstart (Übersicht)
1. Repo klonen
2. `config.yaml` anlegen und Secrets eintragen
3. Mit Docker starten: `docker compose up -d`
4. Admin unter `http://127.0.0.1:8000` öffnen
5. Account verbinden und Client-Key erstellen

## Hinweise
- Nutze es nur im Rahmen der Grok-Nutzungsbedingungen und geltender Gesetze.
- Es handelt sich um ein Proxy/Gateway, das Accounts und Zugänge verwaltet.

## Wann dieser Skill genutzt werden soll
- Nutzer fragt, was grok2api ist
- Nutzer will wissen, wie man es grob einrichtet
- Nutzer vergleicht es mit offiziellen Grok-APIs

## Vorgehen
1. Kurz und mit Tabelle erklären.
2. Link zum Repo geben.
3. Bei Bedarf den Schnellstart oder einzelne Features genauer beschreiben.
4. Auf Nutzungsbedingungen hinweisen.
