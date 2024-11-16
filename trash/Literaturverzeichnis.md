## Internetquellen
```dataview
TABLE titel, file.etags, length(file.inlinks) AS Backlinks
FROM #literatur/internetquelle 
WHERE file.name != "Internetquelle"
```
