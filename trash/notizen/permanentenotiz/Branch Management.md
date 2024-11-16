---
titel: Branch Management
timestamp: 2024-11-15 19-11-53
tags: notiztyp/permanentenotiz, status/done
---
## Fragestellung
Wie kann Git Branches managen?

## Branch Management
Branches lassen sich mit dem Befehl `branch` managen. Der Befehl bezieht sich immer auf  **aktiven Branch**.

### `git branch --merged`

- Zeigt alle lokalen Branches an, deren Änderungen bereits in den aktuellen Branch zusammengeführt (gemerged) wurden.
- Diese Branches können sicher gelöscht werden, da ihre Änderungen bereits im aktuellen Branch enthalten sind und kein Verlust von Änderungen zu erwarten ist.
- Beispiel: Wenn du auf `main` bist und `git branch --merged` ausführst, listet es alle Branches auf, die bereits in `main` integriert wurden.

### `git branch --no-merged`

- Zeigt alle lokalen Branches an, die noch **nicht** in den aktuellen Branch zusammengeführt wurden.
- Diese Branches enthalten also Änderungen, die noch nicht im aktuellen Branch integriert sind und möglicherweise noch benötigt oder überprüft werden müssen, bevor sie gemerged oder gelöscht werden.
- Beispiel: Wenn du auf `main` bist und `git branch --no-merged` ausführst, listet es alle Branches auf, die noch nicht in `main` integriert sind.


## Gedanken/Reflexion
Wie finde ich raus welcher [[Branch]] wann in den aktuellen [[Branch]] gemergt wurde und wie sieht die [[Commit Id]] aus? [[Merge punkte finden]]

---
*Zentralverzeichnisse:*
[[Keine Zentralverzeichnise]]

*Literaturverweise:*
[[Keine Literaturnotiz]]

*Schlagwörter:*
[[Git]], [[Branch]], [[Management]]