# git cola

> 洗練された直感的なユーザーインターフェースを備えた高機能なGit GUI。
> 詳細情報: <https://git-cola.readthedocs.io/en/latest/git-cola.html>。

- GUIを起動する:

`git cola`

- コミット修正モードでGUIを起動する:

`git cola --amend`

- Gitリポジトリの入力を求める (既定は現在のディレクトリ):

`git cola --prompt`

- 指定したパスにあるGitリポジトリを開く:

`git cola {{[-r|--repo]}} {{Gitリポジトリへのパス}}`

- 状態ウィジェットにパスフィルターを適用する:

`git cola {{[-s|--status-filter]}} {{フィルター}}`
