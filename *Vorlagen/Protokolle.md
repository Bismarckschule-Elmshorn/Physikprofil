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

%% Skizze %%
![[<% tp.file.cursor(1) %>]]

# Aufbau
<% tp.file.cursor(2) %>

# Durchführung
<% tp.file.cursor(3) %>

# Messwerte
| <% tp.file.cursor(4) %> |     |     |
| ----------------------- | --- | --- |
|                         |     |     |

# Beobachtung
<% tp.file.cursor(5) %>

# Auswertung
<% tp.file.cursor(6) %>

# Diskussion
<% tp.file.cursor(7) %>
