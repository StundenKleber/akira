---
titel: <% `${tp.file.title}` %>
timestamp: <% tp.date.now("YYYY-MM-DD HH-MM-ss") %>
tags: notiztyp/permanentenotiz, status/entwurf
aliases:
---
<% 
await tp.file.move(`notizen/permanentenotiz/${tp.file.title}`)
%>
## Fragestellung

## Titel

## Gedanken/Reflexion

---
*Zentralverzeichnisse:*
[[Keine Zentralverzeichnise]]

*Literaturverweise:*

*Schlagwörter:*
[[Keine Schlagwörter]]
