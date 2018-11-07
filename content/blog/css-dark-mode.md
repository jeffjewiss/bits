---
title: "CSS Dark Mode"
date: 2018-11-07T13:15:00-05:00
draft: false
tags:
- css
---

You won't be able to use this just yet as it's only available in the Safari Tech Preview, but a media query for "Dark Mode" will soon be available. Combining the media query with custom variables makes for some pretty easy theming options.


```css
body {
  background-color: var(--background-colour);
  color: var(--text-colour);

}

@media(prefers-color-scheme: dark) {
  :root {
    --background-colour: #111;
    --text-colour: #eee;
  }
}
``````
