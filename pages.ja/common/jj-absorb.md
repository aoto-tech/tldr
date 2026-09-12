# jj absorb

> ソース リビジョン内の変更を分割し、対応する行が最後に変更された最も近い変更可能な祖先に各変更を移動します。
> 祖先リビジョンに一致する領域が 0 個または複数ある変更は移動されません。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-absorb>。

- 適格で明確な変更をすべて、あるリビジョンから他のリビジョンに自動的に移動します:

`jj absorb {{[-f|--from]}} {{revset}} {{[-t|--into]}} {{revsets}}`

- 指定されたファイルの変更のみをあるリビジョンから他のリビジョンに移動します:

`jj absorb {{[-f|--from]}} {{revset}} {{[-t|--into]}} {{revsets}} {{filesets}}`
