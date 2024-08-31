<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");  
  } 
  const modTitle = title.replace(/-/g, " ")

_%>
---
layout: post
	title: <% modTitle %>
comments: false
---