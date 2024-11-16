<%*
const title = await tp.system.prompt("Titel der Notiz")

const source_note = await tp.system.prompt("Quellen-Notiz-Link (z.B., [[Quelle - Titel]])")

await tp.file.move(`notizen/literaturzettel/${title}`)
-%>

---
title:  Literaturzettel - <% title %>
timestamp: <% tp.date.now("YYYY-MM-DD HH-mm-ss") %>
tags: literaturzettel, status/entwurf

---

**Quelle:** <% source_note %>  

**Zusammenfassung/Notizen:**  
- Wesentliche Gedanken oder Anmerkungen zur Quelle.

**Zitate:**  
> Relevantes Zitat oder Textausschnitt.

**Verlinkte Notizen:**  
- [[Weitere verwandte Notizen]]


%%
**Zweck**: Ein Literaturzettel verweist auf eine zentrale Quellen-Notiz und enthält spezifische Gedanken, Zitate oder Anmerkungen zu dieser Quelle. Hier werden persönliche Eindrücke oder Erkenntnisse zur Quelle festgehalten.
%%
