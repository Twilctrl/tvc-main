# tvc-main

A home for projects built with my local models. Local model work is the main focus here, with Claude and Codex projects included as side hobbies.

| Folder          | What's in it              | Source                                                          |
|-----------------|---------------------------|-----------------------------------------------------------------|
| `local-models/` | Main projects built with local models | [Ministral-3-3B Locally](local-models/Ministral-3-3B%20Locally/)|
| `claude/`       | Claude side projects      | [Twilctrl/Claude-Main](https://github.com/Twilctrl/Claude-Main)   |
| `codex/`        | Codex side projects       | [Twilctrl/ChatGPT-Main](https://github.com/Twilctrl/ChatGPT-Main) |

<!-- Keep links to every project folder stored in this repo in the local-models Source cell above. Add each new folder there when it is created. -->

Local model projects live directly in `local-models/`.

`claude/` and `codex/` are git submodules: links to the original repos, not copies.
Keep working on those side projects in their own repos; this one points at a specific commit of each.

## Clone

```sh
git clone --recursive https://github.com/Twilctrl/tvc-main.git
```

Already cloned without `--recursive`?

```sh
git submodule update --init
```

## Update the side-project submodules

To pick up new commits from Claude-Main and ChatGPT-Main:

```sh
git submodule update --remote
git commit -am "Bump submodules"
git push
```
