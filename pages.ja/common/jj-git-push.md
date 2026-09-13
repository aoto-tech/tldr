# jj git push

> Git リモートにプッシュします。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-git-push>。

- ブックマークを指定されたリモートにプッシュします:

`jj git push {{[-b|--bookmark]}} {{bookmark}} --remote {{remote}}`

- 新しいブックマークをプッシュします:

`jj git push {{[-b|--bookmark]}} {{bookmark}} {{[-N|--allow-new]}}`

- 追跡されているすべてのブックマークをプッシュします:

`jj git push --tracked`

- すべてのブックマーク (新しいブックマークを含む) をプッシュします:

`jj git push --all`

- 指定されたリビジョンを指すすべてのブックマークをプッシュします:

`jj git push {{[-r|--revisions]}} {{revset}}`

- 新しいブックマークを作成して変更/コミットをプッシュします (名前の形式は `templates.git_push_bookmark` 設定に従い、デフォルトは `"push-" ++ change_id.short()` です):

`jj git push {{[-c|--change]}} {{revset}}`

- 指定した名前でリビジョンを指すブックマークを作成し、リモートにプッシュします:

`jj git push --named {{name}}={{revision}}`
