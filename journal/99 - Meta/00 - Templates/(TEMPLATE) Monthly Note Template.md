---
date: <% tp.date.now("YYYY-MM-DD") %>
tags: month
cssclasses: dashboard

---
# <% tp.date.now("MMMM YYYY") %>
## Monthly Review
###### << [[<% tp.date.now("MM - MMMM YYYY", "P-1M", tp.file.title, "MM - MMMM YYYY") %>|<% tp.date.now("MMMM YYYY", "P-1M", tp.file.title, "MMMM YYYY") %>]] - [[<% tp.date.now("MM - MMMM YYYY", "P1M", tp.file.title, "MM - MMMM YYYY") %>|<% tp.date.now("MMMM YYYY", "P1M", tp.file.title, "MMMM YYYY") %>]] >>

---
### Highlights
#### Monthly Highlights

#### Daily Highlights
```dataview
TABLE WITHOUT ID link(file.link, dateformat(file.day, "MMMM, dd")) as "Date", join(highlight, "

") as "Highlights"
FROM "03 - Daily Notes"
WHERE file.day.year = this.file.day.year
AND file.day.month = this.file.day.month
AND highlight != null
SORT date
```
---
### Notes
- #### Thoughts
`$=dv.list(dv.pages('"02 - Thoughts"').where(p => p.date?.year == <% tp.date.now("YYYY") %>).where(p => p.date?.month == <% tp.date.now("M") %>).sort(p => p.date).file.link)`
- #### Events
`$=dv.list(dv.pages('"01 - Events"').where(p => p.date?.year == <% tp.date.now("YYYY") %>).where(p => p.date?.month == <% tp.date.now("M") %>).sort(p => p.date).file.link)`
- #### Daily Notes
`$=dv.list(dv.pages('"03 - Daily Notes"').where(p => p.date?.year == <% tp.date.now("YYYY") %>).where(p => p.date?.month == <% tp.date.now("M") %>).sort(p => p.date).file.link)`