# tvc-main

Everything in one place.

| Folder          | What's in it              | Source                                                          |
|-----------------|---------------------------|-----------------------------------------------------------------|
| `claude/`       | Claude projects           | [Twilctrl/Claude-Main](https://github.com/Twilctrl/Claude-Main)   |
| `codex/`        | Codex projects            | [Twilctrl/ChatGPT-Main](https://github.com/Twilctrl/ChatGPT-Main) |
| `local-models/` | Local model projects      | This repo                                                       |

`claude/` and `codex/` are git submodules: links to the original repos, not copies.
Keep working in those repos; this one points at a specific commit of each.

## Clone

```sh
git clone --recursive https://github.com/Twilctrl/tvc-main.git
```

Already cloned without `--recursive`?

```sh
git submodule update --init
```

## Pick up new commits from Claude-Main / ChatGPT-Main

```sh
git submodule update --remote
git commit -am "Bump submodules"
git push
```
