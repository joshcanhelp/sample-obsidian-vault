---
status: now
status_note: Finish updating resume
---

- [ ] [[Working/New Job|New Job]] - Finish resume edits
- [ ] [[Working/New Job|New Job]] - Email [[People/Alice|Alice]] from [[Organizations/Sample Organization|Sample Organization]]
##### Companies

```dataview
TABLE glassdoor_score AS "Score", file.mday AS "Modified"
FROM "Organizations"
WHERE candidate
SORT glassdoor_score DESC, file.mday DESC
```

##### Logs
```dataview
LIST
FROM "Logs"
WHERE project 
	AND contains(project, this.file.link)
SORT file.name DESC
```