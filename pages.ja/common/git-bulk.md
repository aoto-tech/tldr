# git bulk

> 複数のGitリポジトリに対して操作を実行する。
> `git-extras` の一部。
> 詳細情報: <https://github.com/tj/git-extras/blob/main/Commands.md#git-bulk>。

- 現在のディレクトリをワークスペースとして登録する:

`git bulk --addcurrent {{ワークスペース名}}`

- 一括操作用のワークスペースを登録する:

`git bulk --addworkspace {{ワークスペース名}} /{{リポジトリへのパス}}`

- 指定したディレクトリ内にリポジトリをクローンし、ワークスペースとして登録する:

`git bulk --addworkspace {{ワークスペース名}} /{{親ディレクトリへのパス}} --from {{リモートリポジトリの場所}}`

- 改行区切りのリモート位置一覧からリポジトリをクローンし、ワークスペースとして登録する:

`git bulk --addworkspace {{ワークスペース名}} /{{ルートディレクトリへのパス}} --from /{{ファイルへのパス}}`

- 登録済みのすべてのワークスペースを一覧表示する:

`git bulk --listall`

- 現在のワークスペースにあるリポジトリでGitコマンドを実行する:

`git bulk {{コマンド}} {{コマンドの引数}}`

- 指定したワークスペースを削除する:

`git bulk --removeworkspace {{ワークスペース名}}`

- すべてのワークスペースを削除する:

`git bulk --purge`
