---
layout: default
title: Submodules & Workspace
parent: Guides
nav_order: 1
---

## Clone
```sh
git submodule update --init --recursive
```

## Pull latest (tracked branches)
```sh
git submodule update --remote --checkout --recursive
```

## Common fixes
- `--checkout` vs `--merge`
- Pin branches in `.gitmodules`
- Reset a submodule
- `git submodule update --init` to reinit

## Workflow
Keep submodules up to date before commits.
