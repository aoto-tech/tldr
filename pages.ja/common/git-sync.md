# git sync

> ローカルブランチをリモートブランチと同期する。
> `git-extras` の一部。
> 詳細情報: <https://manned.org/git-sync>。

- 現在のローカルブランチを対応するリモートブランチと同期する:

`git sync`

- 現在のローカルブランチをリモートのmainブランチと同期する:

`git sync origin main`

- 追跡されていないファイルを削除せずに同期する:

`git sync {{[-s|--soft]}} {{リモート名}} {{ブランチ名}}`
