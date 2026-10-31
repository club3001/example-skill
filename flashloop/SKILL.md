---
name: flashloop-explainer
description: "Erklärt FlashLoop einfach und verständlich. Nutzen wenn der Nutzer nach FlashLoop, Looped Transformers, effizienter Inferenz oder flashloop_torch fragt."
type: knowledge
lifecycle: active
---

# FlashLoop — Einfache Erklärung

FlashLoop macht bestimmte KI-Modelle (Looped Transformers) schneller und speichereffizienter – ohne sie neu zu trainieren.

## Was sind Looped Transformers?
Normale Transformers durchlaufen ihre Schichten einmal.  
Looped Transformers wenden denselben Block **mehrfach hintereinander** an (mehr „Tiefe“ ohne mehr Parameter).  
Das kostet aber mehr Rechenzeit und Speicher (besonders den KV-Cache).

## Was FlashLoop macht
Es erkennt, dass in späteren Loops viele Tokens sich kaum noch ändern. Deshalb:
- Nur „aktive“ Tokens werden neu berechnet (token-sparse updates)
- Attention wird sparsamer gemacht
- Der KV-Cache wird komprimiert

Ergebnis (laut Paper): bis zu ca. 1.6× schneller und bis zu 6× weniger Speicher.

## Die zwei Versionen
| Paket | Zweck |
|-------|------|
| `flashloop` | Optimierte CUDA-Version (schnell) |
| `flashloop_torch` | Lesbare PyTorch-Version zum Verstehen und Experimentieren |

Typische Nutzung der PyTorch-Version:
```python
from flashloop_torch import flashloop

with flashloop(model) as hooks:
    output = model.generate(...)
```

## Wann dieser Skill genutzt werden soll
- Nutzer fragt, was FlashLoop ist
- Nutzer zeigt Dateien aus dem FlashLoop-Repo (z. B. `flashloop_torch/__init__.py`)
- Nutzer will den Unterschied zwischen normalem Transformer und Looped Transformer verstehen

## Vorgehen
1. Kurz und einfach erklären (Tabelle nutzen).
2. Bei Bedarf den Unterschied der beiden Pakete zeigen.
3. Anbieten, das offizielle Repo zu öffnen oder ein Beispiel zu erklären.

Repo: https://github.com/Superone77/FlashLoop
