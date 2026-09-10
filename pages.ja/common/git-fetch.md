# git fetch

> リモートリポジトリからオブジェクトと参照をダウンロードする。
> 詳細情報: <https://git-scm.com/docs/git-fetch>。

- 設定されている場合、既定の上流リモートリポジトリから最新の変更を取得する:

`git fetch`

- 指定した上流リモートリポジトリから新しいブランチを取得する:

`git fetch {{リモート名}}`

- すべての上流リモートリポジトリから最新の変更を取得する:

`git fetch --all`

- 上流リモートリポジトリからタグも取得する:

`git fetch {{[-t|--tags]}}`

- 上流で削除されたリモートブランチへのローカル参照を削除する:

`git fetch {{[-p|--prune]}}`

- 現在の浅いブランチを2コミット分深くする:

`git fetch --deepen 2`

- ブランチを切り替えずに `main` ブランチを更新する (`git pull` と同等):

`git fetch {{origin}} main:main`
