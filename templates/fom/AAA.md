<%*

let file = app.workspace.getActiveFile(); 

console.log(file)

tp.app.fileManager.processFrontMatter(file, (frontmatter) =>{ 

	let res = frontmatter.autor.map(a => (a.nachname || "ERROR") + ', ' + (a.vorname[0]) + '.' || "ERROR").join(", ")

	res = res + ' (' + frontmatter.erscheinungsjahr + '): ' || "( ERROR ): "
	res = res + frontmatter.titel + ", "
	res = res + frontmatter.auflage +". Aufl., "
	res = res + frontmatter.erscheinungsort +" "
	res = res + frontmatter.erscheinungsjahr
	frontmatter["literatureintrag"] = res
});
%>