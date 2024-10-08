##### Now

- [ ] Something that just needs to get done
- [ ] Something else ...

##### Projects
```dataview
TABLE status_note AS Status
WHERE file.folder = "Working" AND status = "now"
```

##### Project TODOs
```dataview
TASK
WHERE !completed AND !checked AND (
file.folder = "Working" OR file.folder = "Events"
)
```
##### Reading + Watching
```dataview
LIST 
FROM "Media"
WHERE status = "waiting"
SORT file.cday ASC
```