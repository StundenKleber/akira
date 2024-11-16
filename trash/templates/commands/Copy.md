<%*
let tags = tp.file.tags
let tagsToCheck = [
"#literatur/internetquelle"
];

let tagExists = tagsToCheck.some(tag => tags.includes(tag));

if(tagExists){
	console.log("Erstelle Literaturnotiz")
	console.log(tp.frontmatter.jahr != null)
}else{
	console.log("Nothing to do!")
}

console.log(tp)
%>
