---
date: <% tp.date.now("YYYY-MM-DD", 0 , tp.file.title, "YYYY") %>
tags: year
cssclasses: dashboard

--- <% await tp.file.move("04 - Yearly Notes/" + tp.file.title) %>
# <% tp.file.title %>
## Year In Review
---
### Highlights
```dataview
TABLE WITHOUT ID file.link as "Month", join(highlight, "

") as "Highlights"
FROM "04 - Monthly Notes"
WHERE file.day.year = this.file.day.year
AND highlight != null
SORT date
```
---