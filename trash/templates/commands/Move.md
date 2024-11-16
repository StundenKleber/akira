<%*
let title = tp.file.title;
// Die aktuelle Datei schließen 
await app.workspace.activeLeaf.detach();
tp.file.move(`/tmp/${title}`)
%>