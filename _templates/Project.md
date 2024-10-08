---
status:
status_note:
organizations:
projects:
---

##### Logs
```dataview
LIST
FROM "Logs"
WHERE project 
	AND contains(project, this.file.link)
SORT file.name DESC
```