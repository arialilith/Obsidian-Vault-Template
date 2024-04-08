---
date: <% tp.date.now("YYYY-MM-DD") %>
subtitle:
type:
subtype:
tags: [thought]
---<% await tp.file.move("02 - Thoughts/" + tp.date.now("YYYY") + "/" + tp.date.now("MM - MMMM YYYY") + "/" + tp.file.title) %>
Tags: #thoughts
Links: [[<% tp.date.now("YYYY-MM-DD") %>]] | [[<% tp.date.now("MM - MMMM YYYY")%>]]

---
# <% tp.file.title %>
<% tp.date.now("YYYY-MM-DD") %>

---
### :TiFileDescription: Description

---
### :BoBxCamera: Pictures