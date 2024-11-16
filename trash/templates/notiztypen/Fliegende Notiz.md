---
titel: <% `~${tp.file.title}` %>
timestamp: <% tp.date.now("YYYY-MM-DD HH-MM-ss") %>
tags: notiztyp/fliegend, status/entwurf
---
<% await tp.file.move(`notizen/fliegende/~${tp.file.title}`) %>



---
*Schlagwörter:*
[[Keine Schlagwörter]]