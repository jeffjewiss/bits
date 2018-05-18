---
title: "Browserlist Last 2 Versions"
date: 2018-05-18T14:33:39+01:00
draft: false
tags:
- css
- javascript
- babel
- postcss
---

This one comes via [James Kyle](https://jamie.build/last-2-versions), who has worked on Yarn and Babel, among [many other things](https://github.com/jamiebuilds).

It’s been recommended to use “last 2 versions” as the configuration for `browserlist` for quite a while now. However, you’ll end up supporting browsers you don’t intend to...forever. Instead, you should use:

```json
"browsers": [
  ">0.25%",
  "not ie 11",
  "not op_mini all"
]
```
