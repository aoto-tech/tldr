# jj git remote

> Git リモートを管理します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-git-remote>。

- すべての Git リモートをリストします:

`jj git remote list`

- Git リモートを追加します:

`jj git remote add {{remote_name}} {{remote_url}}`

- 特定のプッシュ URL を使用して Git リモートを追加します:

`jj git remote add --push-url {{push_url}} {{remote_name}} {{remote_url}}`

- Git リモートの URL を変更します:

`jj git remote set-url {{remote_name}} {{remote_url}}`

- Git リモートのプッシュ URL を設定します:

`jj git remote set-url --push {{push_url}} {{remote_name}}`

- Git リモートのフェッチ URL とプッシュ URL の両方を設定します:

`jj git remote set-url --fetch {{fetch_url}} --push {{push_url}} {{remote_name}}`

- Git リモートを削除します:

`jj git remote remove {{remote_name}}`

- Git リモートの名前を変更します:

`jj git remote rename {{old_name}} {{new_name}}`
