---
titel: <% `${tp.file.title}` %>
timestamp: <% tp.date.now("YYYY-MM-DD HH-MM-ss") %>
tags: notiztyp/permanentenotiz, status/entwurf
---
<% 
await tp.file.move(`notizen/permanentenotiz/${tp.file.title}`)
%>
**Fragestellung**

**Inhalt**

**Gedanken/Reflexion**

---
*Zentralverzeichnisse:*
[[Kein Zentralverzeichnis]]

*Literaturverweise:*

*Tags:*
