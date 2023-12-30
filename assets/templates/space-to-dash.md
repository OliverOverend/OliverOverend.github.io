<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");  
  } 
  const modTitle = title.replace(/ /g, "-").toLowerCase()

  await tp.file.rename(modTitle)
_%>
---
layout: post
title:  <% modTitle %>
---