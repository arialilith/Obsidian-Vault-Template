---
date: <% tp.date.now("YYYY-MM-DD") %>
cssclass: events
subtitle:
type:
subtitle:
tags: [event]
---<% await tp.file.move("03 - Permanent/Events/" + tp.date.now("YYYY") + "/" + tp.date.now("MM - MMMM YYYY") + "/" + tp.file.title) %>
# [[<% tp.file.title %>]]
## [[<% tp.date.now("YYYY-MM-DD") %>|<% tp.date.now("MMMM Do, YYYY") %>]]

---
### :TiFileDescription: Description


---
### :BoBxCamera: Pictures

---
###### Links: [[<% tp.date.now("YYYY-MM-DD") %>]] | [[<% tp.date.now("MM - MMMM YYYY")%>]]