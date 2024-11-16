<%*
const title = await tp.system.prompt("Titel der Quelle")
const author = await tp.system.prompt("Autor(en)")
const year = await tp.system.prompt("Veröffentlichungsjahr")
const type = await tp.system.suggester(["Monographie", "Aufsatz/Artikel in Sammelwerk", "Zeitschriftenartikel", "Internetquelle", "ChatGPT"], ["Monographie", "Aufsatz/Artikel in Sammelwerk", "Zeitschriftenartikel", "Internetquelle", "ChatGPT"])

let publisher = ""
let location = ""
let journal = ""
let volume = ""
let issue = ""
let pages = ""
let url = ""
let access_date = ""
let editor = ""

if (type == "Monographie") {
  publisher = await tp.system.prompt("Verlag")
  location = await tp.system.prompt("Erscheinungsort")
} else if (type == "Aufsatz/Artikel in Sammelwerk") {
  editor = await tp.system.prompt("Herausgeber des Sammelwerks")
  publisher = await tp.system.prompt("Verlag")
  location = await tp.system.prompt("Erscheinungsort")
  pages = await tp.system.prompt("Seitenbereich")
} else if (type == "Zeitschriftenartikel") {
  journal = await tp.system.prompt("Zeitschrift/Zeitung")
  volume = await tp.system.prompt("Band/Volume")
  issue = await tp.system.prompt("Ausgabe/Issue")
  pages = await tp.system.prompt("Seitenbereich")
} else if (type == "Internetquelle") {
  url = await tp.system.prompt("URL")
  access_date = await tp.system.prompt("Zugriffsdatum")
} else if (type == "ChatGPT") {
  access_date = await tp.system.prompt("Datum des Gesprächs")
}
-%>

---
title: "<% title %>"
author: "<% author %>"
year: "<% year %>"
type: "<% type %>"
tags: Quelle, <% type %>, status/entwurf
<%* if (type == "Monographie") { %>
publisher: "<% publisher %>"
location: "<% location %>"
<%* } else if (type == "Aufsatz/Artikel in Sammelwerk") { %>
editor: "<% editor %>"
publisher: "<% publisher %>"
location: "<% location %>"
pages: "<% pages %>"
<%* } else if (type == "Zeitschriftenartikel") { -%>
journal: "<% journal %>"
volume: "<% volume %>"
issue: "<% issue %>"
pages: "<% pages %>"
<%* } else if (type == "Internetquelle") { -%>
url: "<% url %>"
access_date: "<% access_date %>"
<%* } else if (type == "ChatGPT") { -%>
access_date: "<% access_date %>"
<%* } -%>
---

**Zusammenfassung:**  
- Kurze Beschreibung oder zentrale Ideen der Quelle.

%%
**Zweck**: Die zentrale Quellen-Notiz dient dazu, alle bibliografischen Details zu einer bestimmten Quelle zu speichern (Autor, Erscheinungsjahr, Verlag, usw.). Diese Informationen werden einmalig erfasst und dann in anderen Notizen, wie den Literaturzetteln, referenziert.
%%
