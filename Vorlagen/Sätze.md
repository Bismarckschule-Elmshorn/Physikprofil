<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(`${title}`);
  } 
%># $<% tp.file.cursor(1) %>$

Der <%* tR += `${title}` %> besagt, dass <% tp.file.cursor(2) %>
