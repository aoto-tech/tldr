# git fetch

> リモートリポジトリからオブジェクトと参照をダウンロードする。
> 詳細情報: <https://git-scm.com/docs/git-fetch>。

- 既定のリモートリポジトリが設定されている場合、その最新の変更を取得する:

`git fetch`

- 指定したリモートリポジトリから新しいブランチを取得する:

`git fetch {{remote_name}}`

- すべてのリモートリポジトリから最新の変更を取得する:

`git fetch --all`

- リモートリポジトリからタグも取得する:

`git fetch {{[-t|--tags]}}`

- upstream で削除されたリモートブランチへのローカル参照を削除する:

`git fetch {{[-p|--prune]}}`

- 現在の shallow ブランチの履歴を2コミット分深くする:

`git fetch --deepen 2`

- `main` ブランチへ切り替えずに更新する (`git pull` と同等):

`git fetch {{origin}} main:main`
