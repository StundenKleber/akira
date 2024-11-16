---
timestamp: <% tp.date.now("YYYY-MM-DD HH-mm-ss") %>
tags: gpt
---
<%* 
const date = tp.date.now("YYYY-MM-DD HH-mm-ss"); 
const newTitle = `GPT ${date}`; 
await tp.file.rename(newTitle);
const newPath = `GptConversations/${newTitle}`;
await tp.file.move(newPath);
%>

## **Frage**


## **Antwort**



---

*Literaturnotiz:*