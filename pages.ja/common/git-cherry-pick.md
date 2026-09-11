# git cherry-pick

> 既存のコミットで導入された変更を現在のブランチに適用する。
> 変更を別のブランチへ適用するには、先に `git checkout` で対象のブランチへ切り替える。
> 詳細情報: <https://git-scm.com/docs/git-cherry-pick>。

- コミットを現在のブランチへ適用する:

`git cherry-pick {{commit}}`

- コミット範囲を現在のブランチへ適用する (`git rebase --onto` も参照):

`git cherry-pick {{start_commit}}~..{{end_commit}}`

- 複数の連続していないコミットを現在のブランチへ適用する:

`git cherry-pick {{commit1 commit2 ...}}`

- コミットを作成せず、コミットの変更だけをワーキングツリーへ追加する:

`git cherry-pick {{[-n|--no-commit]}} {{commit}}`

- cherry-pick されたことを示す行をコミットメッセージに追加する:

`git cherry-pick -x {{commit}}`
