---
titel: <% `${tp.file.title}` %>
timestamp: <% tp.date.now("YYYY-MM-DD HH-MM-ss") %>
tags: schlagwort
aliases:
---
<% 
await tp.file.move(`schlagworte/${tp.file.title}`)
%>