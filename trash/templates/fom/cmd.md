<%*
let autor = tp.frontmatter.autor
let res = ""

console.log(autor)

if(autor && Array.isArray(autor) ){
	res = autor.map(a => (a?.nachname || "ERROR") + ', ' + (a?.vorname[0]) + '.' || "ERROR").join(", ")

	

}else{
	res="No autor"
}
%><% res %>