# jj split

> リビジョンを 2 つに分割します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-split>。

- 指定されたリビジョンを対話的に 2 つに分割し、2 番目のリビジョンをその上に置きます:

`jj split {{[-r|--revision]}} {{revision}}`

- 指定されたリビジョンから一致するファイルを分割します:

`jj split {{[-r|--revision]}} {{revision}} {{fileset}}`

- 指定されたリビジョンを分割し、2 番目のリビジョンを指定された宛先の上に置きます:

`jj split {{[-r|--revision]}} {{revision}} {{[-d|--destination]}} {{revset}}`

- 指定されたリビジョンを分割し、2 番目のリビジョンを他のリビジョンの前または後に配置します:

`jj split {{[-r|--revision]}} {{revision}} {{[-B|--insert-before]}} {{revset}} {{[-A|--insert-after]}} {{revset}}`

- 指定されたリビジョンを 2 つの並列リビジョンに分割します:

`jj split {{[-r|--revision]}} {{revision}} {{[-p|--parallel]}}`
