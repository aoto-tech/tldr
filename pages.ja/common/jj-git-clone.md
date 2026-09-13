# jj git clone

> Git リポジトリのクローンを基にした新しいリポジトリを作成します。
> 注: `--colocate` が使用されない限り、それは有効な Git リポジトリではないため、`git` コマンドは使用できません。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-git-clone>。

- Git リポジトリのクローンを基にした新しいリポジトリを指定されたディレクトリに作成します:

`jj git clone {{source}} {{path/to/directory}}`

- クローンを作成し、新しく作成したリモートに指定された名前を使用します:

`jj git clone --remote {{remote_name}} {{source}}`

- Git リポジトリのクローンを作成し、最新の 10 件のコミットのみを取得します:

`jj git clone --depth {{10}} {{source}}`

- Jujutsu リポジトリを Git リポジトリと同じ場所に配置するクローンを作成します (同じディレクトリ内で `jj` と `git` コマンドの両方を使用できるようにします):

`jj git clone --colocate {{source}}`
