# docker search

> Docker Hub で Docker イメージを検索します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/search/>。

- 名前またはキーワードで Docker イメージを検索します:

`docker search {{keyword}}`

- 画像を検索し、公式のもののみを表示します:

`docker search {{[-f|--filter]}} is-official=true {{keyword}}`

- イメージを検索し、自動化されたビルドのみを表示します:

`docker search {{[-f|--filter]}} is-automated=true {{keyword}}`

- 星の数が最小の画像を検索します:

`docker search {{[-f|--filter]}} stars={{number}} {{keyword}}`

- 結果の数を制限します:

`docker search --limit {{number}} {{keyword}}`

- 出力形式をカスタマイズします:

`docker search {{[-f|--format]}} "{{.Name}}: {{.Description}}" {{keyword}}`
