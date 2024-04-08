---
date: 3000-01-01
cssclass: dashboard
tags: event

---
# All Events
- #### 2023
`$=dv.list(dv.pages('#event').where(p => p.date?.year == 2023).sort(p => p.date).file.link)`
- #### 2024
`$=dv.list(dv.pages('#event').where(p => p.date?.year == 2024).sort(p => p.date).file.link)`