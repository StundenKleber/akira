<%*
await app.workspace.activeLeaf.detach();

let r = tp.app.vault.getAllLoadedFiles()
  .filter(x => x instanceof tp.obsidian.TFolder)
  .map(x => x.name)

console.log(r)
%>


