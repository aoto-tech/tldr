# docker container commit

> コンテナーの変更から新しいイメージを作成します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/container/commit/>。

- 特定のコンテナからイメージを作成します:

`docker {{[commit|container commit]}} {{container}} {{image}}:{{tag}}`

- 作成したイメージに `CMD` Dockerfile 命令を適用します:

`docker {{[commit|container commit]}} {{[-c|--change]}} "CMD {{command}}" {{container}} {{image}}:{{tag}}`

- 作成したイメージに `ENV` Dockerfile 命令を適用します:

`docker {{[commit|container commit]}} {{[-c|--change]}} "ENV {{name}}={{value}}" {{container}} {{image}}:{{tag}}`

- メタデータに特定の作成者を含む画像を作成します:

`docker {{[commit|container commit]}} {{[-a|--author]}} "{{author}}" {{container}} {{image}}:{{tag}}`

- メタデータに特定のコメントを含む画像を作成します:

`docker {{[commit|container commit]}} {{[-m|--message]}} "{{comment}}" {{container}} {{image}}:{{tag}}`

- コミット中にコンテナを一時停止せずにイメージを作成します:

`docker {{[commit|container commit]}} {{[-p|--pause]}} false {{container}} {{image}}:{{tag}}`

- ヘルプを表示する:

`docker {{[commit|container commit]}} --help`
