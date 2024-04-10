---
cssclass: dashboard
tags:
---
# Aria's Notes
---
### To-Do List
```dataviewjs
dv.taskList(dv.pages('"05 - Journal/Daily Notes"').file.tasks 
  .where(t => !t.completed))
```
---
### Important Links
- #### Spreadsheets
- #### Google
	- [Google Calendar](https://calendar.google.com/calendar/u/0/r)
	- [Google Photos](https://photos.google.com/)

---
### Notes
- #### Homepages
`$=dv.list(dv.pages('#homepage').file.link)`
- #### Monthly Notes
`$=dv.list(dv.pages('#month').sort(f => f.file.name, "desc").limit(4).file.link)`
- #### Yearly Notes
`$=dv.list(dv.pages('#year').sort(f => f.file.name, "desc").limit(3).file.link)`
- #### Events
`$=dv.list(dv.pages('#event').sort(f => f.file.day, "desc").limit(4).file.link)`
- #### Thoughts
`$=dv.list(dv.pages('#thought').sort(f => f.file.day, "desc").limit(4).file.link)`
- #### Recent Files
`$=dv.list(dv.pages('').sort(f => f.file.mtime.ts, "desc").limit(5).file.link)`
---