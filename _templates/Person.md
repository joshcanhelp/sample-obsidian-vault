---
link_to: 
linkedin: 
github: 
twitter: 
organizations:
---

##### Logs
```dataview
LIST WITHOUT ID file.link
FROM "Logs"
WHERE people 
	AND contains(people, this.file.link)
SORT file.name DESC
```