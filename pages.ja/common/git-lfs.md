# git lfs

> Gitリポジトリ内の大容量ファイルを扱う。
> 詳細情報: <https://github.com/git-lfs/git-lfs/tree/main/docs>。

- Git LFSを初期化する:

`git lfs install`

- globに一致するファイルを追跡する:

`git lfs track '{{*.bin}}'`

- Git LFSのエンドポイントURLを変更する (LFSサーバーがGitサーバーと異なる場合に便利):

`git config {{[-f|--file]}} .lfsconfig lfs.url {{LFSエンドポイントURL}}`

- 追跡中のパターンを一覧表示する:

`git lfs track`

- コミット済みの追跡対象ファイルを一覧表示する:

`git lfs ls-files`

- すべてのGit LFSオブジェクトをリモートサーバーへプッシュする (エラーが発生した場合に便利):

`git lfs push --all {{リモート名}} {{ブランチ名}}`

- すべてのGit LFSオブジェクトを取得する:

`git lfs fetch`

- ポインターファイルを実際のGit LFSオブジェクトに置き換える:

`git lfs checkout`
