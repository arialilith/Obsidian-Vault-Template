---
date: <% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "MM - MMMM YYYY") %>
tags: month
cssclasses: dashboard

--- <% await tp.file.move("05 - Journal/Monthly Notes/" + tp.date.now("YYYY", 0, tp.file.title, "MM - MMMM YYYY") + "/" + tp.file.title) %>

# <% tp.date.now("MMMM YYYY", 0, tp.file.title, "MM - MMMM YYYY") %>

## Monthly Review
##### << [[<% tp.date.now("MM - MMMM YYYY", "P-1M", tp.file.title, "MM - MMMM YYYY") %>|<% tp.date.now("MMMM YYYY", "P-1M", tp.file.title, "MMMM YYYY") %>]] - [[<% tp.date.now("MM - MMMM YYYY", "P1M", tp.file.title, "MM - MMMM YYYY") %>|<% tp.date.now("MMMM YYYY", "P1M", tp.file.title, "MMMM YYYY") %>]] >>
##### [[<% tp.date.now("YYYY", 0, tp.file.title, "MM - MMMM YYYY") %>|View <% tp.date.now("YYYY", 0, tp.file.title, "MM - MMMM YYYY") %>]]

---
### Highlights
#### Monthly Highlights

#### Daily Highlights
```dataview
TABLE WITHOUT ID link(file.link, dateformat(file.day, "MMMM, dd")) as "Date", join(highlight, "

") as "Highlights"
FROM "05 - Journal/Daily Notes"
WHERE file.day.year = this.file.day.year
AND file.day.month = this.file.day.month
AND highlight != null
SORT date
```
---
### Notes
- #### Thoughts
`$=dv.list(dv.pages('"03 - Permanent/Thoughts"').where(p => p.date?.year == <% tp.date.now("YYYY", 0, tp.file.title, "MM - MMMM YYYY") %>).where(p => p.date?.month == <% tp.date.now("M", 0, tp.file.title, "MM - MMMM YYYY") %>).sort(p => p.date).file.link)`
- #### Events
`$=dv.list(dv.pages('"03 - Permanent/Events"').where(p => p.date?.year == <% tp.date.now("YYYY", 0, tp.file.title, "MM - MMMM YYYY") %>).where(p => p.date?.month == <% tp.date.now("M", 0, tp.file.title, "MM - MMMM YYYY") %>).sort(p => p.date).file.link)`
- #### Daily Notes
`$=dv.list(dv.pages('"05 - Journal/Daily Notes"').where(p => p.date?.year == <% tp.date.now("YYYY", 0, tp.file.title, "MM - MMMM YYYY") %>).where(p => p.date?.month == <% tp.date.now("M", 0, tp.file.title, "MM - MMMM YYYY") %>).sort(p => p.date).file.link)`
---
###### Links: [[<%tp.date.now("YYYY",0,tp.file.title, "MM - MMMM YYYY")%>]]