<%*
const title = await tp.system.prompt("Titel des Oberthemas")
await tp.file.move(`notizen/(Themenzettel) ${title}`)
-%>
---
title: Themenzettel - <% title %>
timestamp: <% tp.date.now("YYYY-MM-DD HH-mm-ss") %>
tags: "themenzettel"

---

**Thema:** <% title %>  

**Überblick:**  
- Beschreibung des Themas und seiner Relevanz.


**Verwendete Literatur:**  
- [[Leerer Verweis|Verweis auf relevante Literaturzettel]]

**Verlinkte Notizen:**  
- [[Leerer Verweis|Referenz auf verwandte Notizen]]


**Verwandte Themen:**  
- [[Leerer Verweis|Referenz auf verwandte Themen]] oder wichtige [[Quellen]].

%%
**Zweck**: Ein Themenzettel bündelt Notizen und Quellen zu einem übergeordneten Thema. Er stellt eine Art Sammlung und Übersicht dar und verweist auf spezifische Notizen und relevante Literaturzettel, die zum Thema gehören.

Ein **Themenzettel** ist spezifischer und konzentriert sich auf ein bestimmtes Thema oder Konzept. Er dient dazu, **Informationen, Notizen und Quellen zu einem bestimmten Thema zusammenzuführen**. Der Themenzettel stellt Zusammenhänge dar und kann als Überblick für dieses spezielle Thema verwendet werden. Er kann Verweise auf relevante Literatur, einzelne Notizzettel und verwandte Themenzettel enthalten.

- **Fokus**: Ein spezifisches Thema (z. B. „Sozialer Wandel“).
- **Inhalt**: Umfasst eine Beschreibung des Themas, relevante Literatur, Notizen und verwandte Themenzettel.
- **Verwendung**: Um tiefere Erkenntnisse zu einem bestimmten Thema zu sammeln und zu strukturieren.
-
**Beispiel für Themenzettel**:  
Der Themenzettel „Sozialer Wandel“ würde Notizen und Literatur zum sozialen Wandel sammeln und erklären, wie sich soziale Normen und Werte verändern, sowie Notizen und Quellen zu spezifischen Aspekten des sozialen Wandels wie Digitalisierung oder Individualisierung verknüpfen.

%%
