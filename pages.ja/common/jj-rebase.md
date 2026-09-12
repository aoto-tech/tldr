# jj rebase

> リビジョンを別の親に移動します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-rebase>。

- 指定されたリビジョンを別の親に移動します:

`jj rebase {{[-r|--revisions]}} {{revset}} {{[-o|--onto]}} {{revset}}`

- 指定されたリビジョンとそのすべての子孫を移動します:

`jj rebase {{[-s|--source]}} {{revset}} {{[-o|--onto]}} {{revset}}`

- 指定されたリビジョンを含むブランチ内のすべてのリビジョンを移動します:

`jj rebase {{[-b|--branch]}} {{revset}} {{[-o|--onto]}} {{revset}}`

- リビジョンを他のリビジョンの前または後に移動します:

`jj rebase {{[-r|--revisions]}} {{revset}} {{[-B|--insert-before]}} {{revset}} {{[-A|--insert-after]}} {{revset}}`
