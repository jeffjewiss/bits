---
title: "iex Config"
date: 2018-05-14T13:25:38+01:00
draft: false
tags:
- elixir
---

Okay, this is a quick one. You’ll probably find yourself jumping in an `iex` REPL quite a bit while working on elixir projects. It can become tedious aliasing your frequently used modules. One way to avoid this is to configure them in an `.iex.exs` file:

```elixir
alias MyApp.{
  Repo,
  User,
  Company
}

import Ecto
import Ecto.Changeset
import Ecto.Query, only: [from: 1, from: 2]
```
