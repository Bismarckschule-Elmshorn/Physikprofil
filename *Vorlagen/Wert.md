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

## <% tp.file.cursor(1) %> $<% tp.file.cursor(2) %>$

<% filename %> ist <% tp.file.cursor(3) %>