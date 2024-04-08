---
cssclass: dashboard
tags:
---
# Aria's Notes
---
### To-Do List
```dataviewjs
dv.taskList(dv.pages('"03 - Daily Notes"').file.tasks 
  .where(t => !t.completed))
```
---
### Important Links
- #### Spreadsheets
	- [Devon x Aria Bucket List](https://docs.google.com/spreadsheets/d/1LuVt7nI7i_dwfdH8-idVhor8Ote92spgLxKZjWDwf8A/edit#gid=0)
	- [Semester Spending](https://docs.google.com/spreadsheets/d/1HLuvqtEkg2tjGBQmG2FvrKhgoUsxKMQ7WaRfXl4TtDs/edit#gid=0)
	- [Shopping List](https://docs.google.com/spreadsheets/d/10p9KcJB2YOWxnwuyJ8aO5owQE5f-zT8zlChiSs_rvOc/edit#gid=0)
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
