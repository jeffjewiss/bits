---
title: "Mix Format"
date: 2018-05-17T12:18:24+01:00
draft: false
tags:
- elixir
---

Following in the footsteps of [Go](https://golang.org/), [Elixir](https://elixir-lang.org/) now has a standard formatter as of Elixir v1.6. Create a file called `.formatter.exs` with the inputs for your project, like this:

```elixir
[
  inputs: [
    "mix.exs",
    "{config,lib,test}/**/*.{ex,exs}"
  ]
]
```

and you can now run `mix format` to format your code in a standard style. An example `.formatter.exs` will be added to new projects created using `mix new`.
