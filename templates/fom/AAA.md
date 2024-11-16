<%*

let file = app.workspace.getActiveFile(); 

console.log(file)

tp.app.fileManager.processFrontMatter(file, (frontmatter) =>{ 

	let res = frontmatter.autor.map(a => (a.nachname + ', ' + (a.vorname[0]) + '.').join(", ")

	res = res + ' (' + frontmatter.erscheinungsjahr + '): ' 
	res = res + frontmatter.titel + ", " 
	res = res + frontmatter.auflage +". Aufl., " 
	res = res + frontmatter.erscheinungsort +" " 
	res = res + frontmatter.erscheinungsjahr 
	
	frontmatter["literatureintrag"] = res
});
%>