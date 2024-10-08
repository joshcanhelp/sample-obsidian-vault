- [\#process](obsidian://search??vault=Notes&query=tag:%23process)
- [[TODO]]
##### Logs
```dataview
LIST
FROM "Logs"
WHERE startswith(file.name, string(date(this.file.name)))
```
##### Created
```dataview
LIST
WHERE file.cday = date(this.file.name)
	AND !startswith(file.folder, "Daily/2")
	AND !startswith(file.name, string(date(this.file.name)))
```
