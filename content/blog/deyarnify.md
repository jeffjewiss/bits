---
title: "Deyarnify"
date: 2018-11-23T14:29:08+01:00
draft: false
tags:
- npm
- yarn
---

With some improvements to NPM and `package-lock.json` files I've been using Yarn
less in apps and packages. The deyarn package is a shortcut to cleanup your
node_modules directory, remove your `yarn.lock` file, and then create a `package-lock.json`.

```
npm install deyarn --global
git checkout -b deyarn
deyarn
```

*Note: A warning will be added to the yarn engine entry in your package.json,
which is fine for applications, but will cause an error if the package is used
as a dependency in a project.*
