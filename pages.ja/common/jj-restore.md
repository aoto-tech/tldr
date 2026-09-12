# jj restore

> 別のリビジョンからファイルを復元します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-restore>。

- ファイルをあるリビジョンから別のリビジョンに復元します:

`jj restore {{[-f|--from]}} {{revset}} {{[-t|--into]}} {{revset}} {{filesets}}`

- 親のマージと比較して、リビジョン内の変更を元に戻します:

`jj restore {{[-c|--changes-in]}} {{revset}} {{filesets}}`

- 復元する部分を対話的に選択します:

`jj restore {{[-f|--from]}} {{revset}} {{[-t|--into]}} {{revset}} {{[-i|--interactive]}}`
