<%*
const title = await tp.system.prompt("Projektname oder Fragestellung")
const start_date = await tp.system.prompt("Startdatum")

await tp.file.move(`notizen/projektzettel/${title}`)
-%>

---
title: Projektzettel - <% title %>
timestamp: <% tp.date.now("YYYY-MM-DD HH-mm-ss") %>
tags: projektzettel, status/entwurf

---

**Projektname:** <% title %>  
**Startdatum:** <% start_date %>  

**Projektziel:**  
- Ziel des Projekts oder der Fragestellung.

**Verwendete Literatur:**  
- [[Verweis auf relevante Literaturzettel]]

**Projektumfang und Aufgaben:**  
- Liste der Aufgaben, die zum Projekt gehören.

**Verknüpfte Notizen und Quellen:**  
- [[Liste der zugehörigen Notizzettel]]

%%
**Zweck**: Der Projektzettel ist für laufende Projekte oder spezifische Fragestellungen gedacht. Er enthält das Projektziel, eine Sammlung zugehöriger Aufgaben und verweist auf relevante Notizen und Quellen, um die Projektarbeit zu strukturieren.
%%
