---
title: "Elixir Git Hooks"
date: 2018-05-15T16:17:22+01:00
draft: false
tags:
- elixir
---

I’ve found it helps to keep code quality up, even on features in progress, by frequently running code linters or formatters, as well as your test suite. Git hooks are a great way to trigger the above and there’s a package for Elixir, which makes the setup trivial for any Mix project.

Once you install [Elixir Git Hooks](https://github.com/qgadrian/elixir_git_hooks) and compile it, you just need to configure which git hooks you’d like to use:


```elixir
config :git_hooks,
  verbose: true,
  hooks: [
    pre_commit: [
      mix_tasks: [
        "format"
      ]
    ],
    pre_push: [
      verbose: false,
      mix_tasks: [
        "test"
      ]
    ]
  ]
```

Now whenever you run the configured git commands the configured mix tasks will run first and must be successful for the git command to succeed.
