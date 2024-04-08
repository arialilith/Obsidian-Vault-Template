---
date: <% tp.file.title %>
tags:
cssclass: daily

---<% await tp.file.move("03 - Daily Notes/2024/" + tp.date.now("MM - MMMM YYYY") + "/" + tp.file.title) %>
# DAILY NOTE
## <% tp.date.now("dddd | MMMM Do, YYYY")%>

###### << [[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>|<% tp.date.now("dddd, MMMM Do", -1, tp.file.title, "YYYY-MM-DD") %>]] - [[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>|<% tp.date.now("dddd, MMMM Do", 1, tp.file.title, "YYYY-MM-DD") %>]] >>

---
### :LiListTodo: To-Do List
- [ ] Write in [[<% tp.file.title %>|daily note]]

---
### :BoBxBookBookmark: Journal
#### Highlights
- 

#### Other Notes
- 

---
Links: [[<% tp.date.now("MMMM YYYY") %>]]