<%*
const title = await tp.system.prompt("Titel der Notiz (z.B., Hauptidee oder Thema)")

await tp.file.move(`notizen/(Notizzettel) ${title}`)
-%>
---
title: Notizzettel - <% title %>
timestamp: <% tp.date.now("YYYY-MM-DD HH-mm-ss") %>
tags: notizzettel, status/entwurf

---

**Hauptgedanke:**  
- Beschreibe den Hauptgedanken prägnant.

**Details und Ausführungen:**  
- Weiterführende Überlegungen, Argumente und Erkenntnisse.

**Verwendete Literatur:**  
- [[Leerer Verweis|Verweis auf relevante Literaturzettel]]

**Verlinkte Notizen:**  
- [[Leerer Verweis|Referenz auf verwandte Notizen]]

**Fragen:**  
- Offene Fragen oder Themen für weitere Recherche.


%%
**Zweck**: Der Notizzettel dient dazu, eigenständige Gedanken und Erkenntnisse festzuhalten, die nicht unbedingt auf einer bestimmten Quelle basieren. Wenn jedoch eine Quelle herangezogen wird, kann der relevante Literaturzettel verlinkt werden.
%%