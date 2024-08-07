---
date: <% tp.date.now("YYYY-MM-DD") %>
cssclass: thoughts
subtitle:
tags: [thought]
---<% await tp.file.move("03 - Permanent/Thoughts/" + tp.date.now("YYYY") + "/" + tp.date.now("MM - MMMM YYYY") + "/" + tp.file.title) %>
# <% tp.file.title %>
## [[<% tp.date.now("MM - MMMM YYYY")%>|<% tp.date.now("MMMM,")%>]] [[<% tp.date.now("YYYY-MM-DD") %>|<% tp.date.now("Do YYYY") %>]]
---

---