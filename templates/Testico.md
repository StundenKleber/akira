<%*
const allTags = new Set(); const files = app.vault.getMarkdownFiles(); 
// Loop through all files and collect tags 
for (const file of files)
{ 

	replaceTag(file,"","")
	
}
function replaceTag(_filename,_seek,_replace){

	const metadata = app.metadataCache.getFileCache(_filename); 
	if(metadata.frontmatter && metadata.frontmatter.tags){
		console.log(metadata.frontmatter.tags)
	}
}
%>