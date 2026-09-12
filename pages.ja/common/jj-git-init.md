# jj git init

> Git をバックエンドとして使用する新しい Jujutsu リポジトリを作成します。
> 注: `--colocate` が使用されない限り、それは有効な Git リポジトリではないため、`git` コマンドは使用できません。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-git-init>。

- 現在のディレクトリに新しい Git ベースのリポジトリを作成します:

`jj git init`

- 指定されたディレクトリに新しい Git ベースのリポジトリを作成します:

`jj git init {{path/to/directory}}`

- Jujutsu リポジトリを有効な Git リポジトリとして初期化します (同じディレクトリ内で `jj` と `git` コマンドの両方を使用できるようにします):

`jj git init --colocate`

- 既存の Git リポジトリを基盤とする Jujutsu リポジトリを初期化します:

`jj git init --git-repo {{git_repo}}`
