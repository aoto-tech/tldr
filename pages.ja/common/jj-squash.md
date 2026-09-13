# jj squash

> 変更をあるリビジョンから別のリビジョンに移動します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-squash>。

- すべての変更を現在のリビジョンからその親に移動します:

`jj squash`

- 指定されたリビジョンからすべての変更をその親に移動します:

`jj squash {{[-r|--revision]}} {{revset}}`

- すべての変更を指定されたリビジョンから指定された他のリビジョンに移動します:

`jj squash {{[-f|--from]}} {{revsets}} {{[-t|--into]}} {{revset}}`

- どの部分を潰すかを対話的に選択します:

`jj squash {{[-i|--interactive]}}`
