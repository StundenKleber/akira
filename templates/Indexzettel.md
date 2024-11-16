<%*
const topic = await tp.system.prompt("Titel des Indexzettels oder Bereichs")
await tp.file.move(`notizen/indexzettel/${title}`)
-%>

---
title: Indexzettel - <% title %>
timestamp: <% tp.date.now("YYYY-MM-DD HH-mm-ss") %>
tags: indexzettel, status/entwurf

---


**Thema:** <% topic %>  

**Zusammenfassung:**  
- Beschreibung und Struktur des Themas.

**Wichtige Themen und Notizen:**  
- [[Verlinkung zu Themenzetteln]] und [[Notizzettel]] für schnellen Zugriff.

**Wichtige Literatur:**  
- Verweise auf zentrale [[Literaturzettel]] für diesen Bereich.

%%
**Zweck**: Der Indexzettel ist eine Art inhaltliches Inhaltsverzeichnis für ein größeres Thema oder eine Kategorie. Er enthält Verweise auf zentrale Themenzettel und wichtige Literatur, um den Überblick über ein Gebiet zu behalten.

Ein **Indexzettel** ist breiter und allgemeiner. Er funktioniert wie ein **Inhaltsverzeichnis** oder eine **Übersicht für ein größeres Themengebiet**. Der Indexzettel verweist auf mehrere Themenzettel und fasst sie unter einem übergeordneten Thema zusammen. Damit ist er eine Metaebene für verschiedene Themen und dient dazu, das große Ganze im Zettelkasten zu organisieren.

- **Fokus**: Ein breites, übergeordnetes Gebiet (z. B. „Gesellschaftliche Strukturen“).
- **Inhalt**: Enthält Verweise auf verschiedene Themenzettel und wichtige Literatur in diesem Bereich.
- **Verwendung**: Um einen umfassenden Überblick über ein großes Themenfeld zu bieten und verschiedene Themenzettel strukturiert zu verlinken.

**Beispiel für Indexzettel**:  
Ein Indexzettel „Gesellschaftliche Strukturen“ würde Themenzettel wie „Sozialer Wandel“, „Moderne Gesellschaft“ und „Kulturwandel“ verlinken und auf wichtige Literatur zu diesen Themen hinweisen, um das gesamte Gebiet der gesellschaftlichen Strukturen zu erschließen.

%%

