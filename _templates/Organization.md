---
link_to: 
careers_link: 
github:
glassdoor_score: 
candidate:
---

##### Logs
```dataview
LIST WITHOUT ID file.link
FROM "Logs"
WHERE organizations 
	AND contains(organizations, this.file.link)
```
##### People
```dataview
LIST
FROM "People"
WHERE organizations 
	AND contains(organizations, this.file.link)
```