---
titel: <% `${tp.file.title}` %>
timestamp: <% tp.date.now("YYYY-MM-DD HH-MM-ss") %>
tags: notiztyp/zentralenotiz, status/entwurf
---

<% 
await tp.file.move(`notizen/zentralenotizen/${tp.file.title}`)
%>

---
*Zentrale Notizen:*

*Schlagwörter:*
[[Keine Schlagwörter]]