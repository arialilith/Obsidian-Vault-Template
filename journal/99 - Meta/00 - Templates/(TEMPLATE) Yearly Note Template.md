---
date: <% tp.date.now("YYYY-MM-DD") %>
tags: year
cssclasses: dashboard
---

# Notes

```dataview
LIST
FROM #bigevent 
WHERE file.ctime.year = [[<%tp.file.title%>]].file.ctime.year
```

```dataview
TABLE WITHOUT ID file.link as "Months"
FROM "journal/daily notes/months"
WHERE file.month = this.file.month
```