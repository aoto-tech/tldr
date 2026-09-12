# jj simplify-parents

> 指定されたリビジョンの親エッジを単純化します。
> たとえば、「A -> B -> C | A -> C」は「A -> B -> C」に簡略化されます。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-simplify-parents>。

- 指定されたリビジョンの親エッジを単純化します:

`jj simplify-parents {{[-r|--revisions]}} {{revsets}}`

- 指定されたリビジョンの親エッジとその子孫のツリーを単純化します:

`jj simplify-parents {{[-s|--source]}} {{revsets}}`
