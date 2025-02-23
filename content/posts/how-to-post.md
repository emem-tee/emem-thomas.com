---
title: "How to Post"
date: 2022-04-11T15:11:17-04:00
draft: true
---

Alrighty, I have managed to fix the issue with not having the Hugo `.exe` file at a location where my shell (I use CMD in Windows) can find it. 

Pro Tip: Do not forget to click `OK` on **ALL** the dialogue boxes in the `System Properties` dialog box. Also make sure you restart your shell when testing.

Now that I have that down, I just have to is navigate to my site's directory (for me that's `.\emem-thomas.com`) and enter the following,

```

hugo new posts/whatever-the-post-is-named.md
REM write some stuff in the markdown file then enter the next line to build your site
hugo -D

```

Then the page should be done. After that, put the corresponding rendered pages onto whatever hosting space you are using. I do not think I put too much thought into my hosting site decision but Hostgator has a lot of information on Youtube and helpful guides. Plus I imagine the price was reasonable (at least it was two or three years ago when I initially subscribed...)