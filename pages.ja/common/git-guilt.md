# git guilt

> 未ステージの変更があるファイルのblame合計数を表示するか、2つのリビジョン間でblameの変化を計算する。
> `git-extras` の一部。
> 詳細情報: <https://manned.org/git-guilt>。

- blameの合計数を表示する:

`git guilt`

- 2つのリビジョン間でblameの変化を計算する:

`git guilt {{最初のリビジョン}} {{最後のリビジョン}}`

- 作成者名の代わりにメールアドレスを表示する:

`git guilt {{[-e|--email]}}`

- blameを割り当てる際に空白だけの変更を無視する:

`git guilt {{[-w|--ignore-whitespace]}}`

- 過去3週間におけるblameの差分を見つける:

`git guilt 'git log --until "3 weeks ago" --format "%H" {{[-n|--max-count]}} 1'`

- 過去3週間におけるblameの差分を見つける (Git 1.8.5以降):

`git guilt @{3.weeks.ago}`
