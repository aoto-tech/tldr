# git filter-repo

> Git履歴を書き換えるための多目的ツール。
> 参照: `bfg`。
> 詳細情報: <https://github.com/newren/git-filter-repo>。

- すべてのファイル内にある機密文字列を置換する:

`git filter-repo --replace-text <(echo '{{検索文字列}}==>{{置換文字列}}')`

- 履歴を保持したまま、1つのフォルダーを抽出する:

`git filter-repo --path {{フォルダーへのパス}}`

- 履歴を保持したまま、1つのフォルダーを削除する:

`git filter-repo --path {{フォルダーへのパス}} --invert-paths`

- サブフォルダー内のすべてを1階層上へ移動する:

`git filter-repo --path-rename {{フォルダーへのパス}}/:`
