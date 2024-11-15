---
titel: <% `${tp.file.title}` %>
timestamp: <% tp.date.now("YYYY-MM-DD HH-MM-ss") %>
tags: notiztyp/literaturnotiz, status/entwurf
---
<% 
await tp.file.move(`notizen/literaturnotizen/${tp.file.title}`)
%>
**Thema oder Kernaussage:**

---
*Quelle:*
[[Keine Quelle]]

*Schlagwörter:*
[[Keine Schlagwörter]]