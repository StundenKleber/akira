```dataview
LIST 
```

```dataview
LIST 
FROM #literatur 
```

```dataview
TABLE titel
FROM #literatur 
```
	
```dataview
TABLE titel
FROM #literatur 
WHERE Txe = "vars"
```
```dataview
TABLE titel, file.etags, file.cday, file.outlinks
FROM #literatur 
WHERE file.frontmatter.titel = "Der Laden"

```


```dataview
TABLE join(list(map(autor, (a) => a.vorname + " " + a.nachname)), ", ") AS "Kombinierte Namen"
FROM #literatur 
WHERE Txe = "vars"
```
```dataview
TABLE join(list(map(autor, (a) => a.vorname + " " + a.nachname)), ", ") AS "Kombinierte Namen", file.inlinks, length(file.inlinks)
FROM #literatur 
WHERE Txe = "vars"
```
## Internetquellen
```dataview
TABLE titel, file.etags, length(file.inlinks) AS Backlinks
FROM #literatur/internetquelle 
WHERE file.name != "Internetquelle"
```

![[Branch Management]]

```dataview
LIST file.folder
FROM #schlagwort 
WHERE file.folder != "templates"
```

```dataview
TABLE file.folder, file.inlinks
FROM #schlagwort 
WHERE file.folder != "templates"
```

<div> hello </div>
<div>world</div>




