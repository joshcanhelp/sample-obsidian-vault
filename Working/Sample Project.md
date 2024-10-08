---
status: now
status_note: Something that reminds me of what's next
organizations:
projects:
---

##### Logs
```dataview
LIST
FROM "Logs"
WHERE projects 
	AND contains(projects, this.file.link)
SORT file.name DESC
```