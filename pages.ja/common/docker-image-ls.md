# docker image ls

> Docker イメージを一覧表示します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/image/ls/>。

- すべての Docker イメージをリストします:

`docker {{[images|image ls]}}`

- 中間を含むすべての Docker イメージをリストします:

`docker {{[images|image ls]}} {{[-a|--all]}}`

- Quiet モードで出力をリストします (数値 ID のみ):

`docker {{[images|image ls]}} {{[-q|--quiet]}}`

- どのコンテナーにも使用されていないすべての Docker イメージをリストします:

`docker {{[images|image ls]}} {{[-f|--filter]}} dangling=true`

- 名前に部分文字列を含むイメージをリストします:

`docker {{[images|image ls]}} "{{*name*}}"`

- 画像をサイズ順に並べ替えます:

`docker {{[images|image ls]}} --format "\{\{.ID\}\}\t\{\{.Size\}\}\t\{\{.Repository\}\}:\{\{.Tag\}\}" | sort {{[-k|--key]}} 2 {{[-h|--human-numeric-sort]}}`
