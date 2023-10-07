---
created: <% tp.date.now("D. MMM. YYYY") %>
aliases:
tags:

---
<%*
let filename = tp.file.title
if (filename.startsWith("Untitled")) {
	filename = await tp.system.prompt("Bitte beginne den Titel mit einem Artikel...")
	await tp.file.rename(filename)
}
_%>

<% filename %> stellt <% tp.file.cursor(1) %> dar.

![[<% tp.file.cursor(2) %>|center|400]]