# jj

> Jujutsu、バージョン管理システム。
> `log`、`desc`、`new`、`git` などの一部のサブコマンドには、独自の使用法ドキュメントがあります。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/>。

- 指定されたリビジョンセット (`B::D`、`A..D`、`B|C|D` など) で指定されたリビジョンの説明を更新します:

`jj {{[desc|describe]}} {{[-m|--message]}} "{{message}}" {{[-r|--revision]}} {{revsets}}`

- 指定されたリビジョンの上に新しいコミット/リビジョンを作成します:

`jj new {{revset}}`

- 複数のリビジョンの上に新しいマージ コミットを作成します:

`jj new {{revset1 revset2 ...}}`

- リビジョンを指すように作業コピーを更新します:

`jj edit {{revset}}`

- 前のコマンド (それ自体が `undo` だった可能性があります) を元に戻します:

`jj undo`

- 作業コピーのスナップショットを作成せずに jj サブコマンドを実行します:

`jj --ignore-working-copy {{subcommand}}`

- 操作時に jj サブコマンドを実行します:

`jj {{[--at-op|--at-operation]}} {{operation}} {{subcommand}}`

- 特定のサブコマンド (`new`、`commit`、`desc` など) のヘルプを表示します:

`jj help {{subcommand}}`
