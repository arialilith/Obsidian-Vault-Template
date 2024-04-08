---
date: <% tp.date.now("YYYY-MM-DD") %>
subtitle:
type:
subtitle:
tags: [event]
---<% await tp.file.move("01 - Events/" + tp.date.now("YYYY") + "/" + tp.date.now("MM - MMMM YYYY") + "/" + tp.file.title) %>
Tags: #event 
Links: [[<% tp.date.now("YYYY-MM-DD") %>]] | [[<% tp.date.now("MM - MMMM YYYY")%>]]

---
# <% tp.file.title %>
<% tp.date.now("YYYY-MM-DD") %>

---
### :TiFileDescription: Description


---
### :BoBxCamera: Pictures