---
date: <% tp.date.now("YYYY-MM-DD") %>
cssclass: thoughts
subtitle:
type:
subtype:
tags: [thought]
---<% await tp.file.move("03 - Permanent/Thoughts/" + tp.date.now("YYYY") + "/" + tp.date.now("MM - MMMM YYYY") + "/" + tp.file.title) %>
# [[<% tp.file.title %>]]
## [[<% tp.date.now("YYYY-MM-DD") %>|<% tp.date.now("MMMM, Do YYYY") %>]]
---

---

###### Links: [[<% tp.date.now("YYYY-MM-DD") %>]] | [[<% tp.date.now("MM - MMMM YYYY")%>]]