---
date: <% tp.file.title %>
tags:
cssclass: daily

---<% await tp.file.move("05 - Journal/Daily Notes/" + tp.date.now("YYYY", 0, tp.file.title, "YYYY-MM-DD") + "/" + tp.date.now("MM - MMMM YYYY", 0, tp.file.title, "YYYY-MM-DD") + "/" + tp.file.title) %>
# DAILY NOTE
## <% tp.date.now("dddd | MMMM Do, YYYY", 0, tp.file.title, "YYYY-MM-DD")%>
##### << [[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>|<% tp.date.now("dddd, Do", -1, tp.file.title, "YYYY-MM-DD") %>]] - [[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>|<% tp.date.now("dddd, Do", 1, tp.file.title, "YYYY-MM-DD") %>]] >>
##### [[<% tp.date.now("MM - MMMM YYYY", 0, tp.file.title, "YYYY-MM-DD")%>|<% tp.date.now("MMMM", 0, tp.file.title, "YYYY-MM-DD")%>]]

---
### :LiListTodo: To-Do List
- [ ] Write in [[<% tp.file.title %>|daily note]]
- [ ] Take pills

---
### :BoBxBookBookmark: Journal
#### Highlights
- 

#### Other Notes
- 

---