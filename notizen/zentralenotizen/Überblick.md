---
titel: Überblick
timestamp: 2024-11-16 14-11-28
tags: notiztyp/zentralenotiz, status/entwurf
---


```dataview
TABLE rows.OUT AS "Unresolved Links" FLATTEN file.outlinks AS OUT WHERE !OUT.file AND !(contains(meta(OUT).path, "/")) GROUP BY file.link AS Source

```



```dataview
TABLE rows.OUT AS Unresolved
FLATTEN file.outlinks AS OUT
WHERE !OUT.file AND !(contains(meta(OUT).path, "."))
GROUP BY file.link AS Source
```
---
*Zentrale Notizen:*

*Schlagwörter:*
[[Keine Schlagwörter]]
