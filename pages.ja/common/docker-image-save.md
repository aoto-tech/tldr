# docker image save

> Docker イメージをアーカイブにエクスポートします。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/image/save/>。

- `stdout` を `.tar` アーカイブにリダイレクトして、画像を保存します:

`docker {{[save|image save]}} {{image}}:{{tag}} > {{path/to/file.tar}}`

- 画像を `.tar` アーカイブに保存します:

`docker {{[save|image save]}} {{[-o|--output]}} {{path/to/file.tar}} {{image}}:{{tag}}`

- 画像のすべてのタグを保存します:

`docker {{[save|image save]}} {{[-o|--output]}} {{path/to/file.tar}} {{image_name}}`

- 画像の特定のタグを厳選して保存します:

`docker {{[save|image save]}} {{[-o|--output]}} {{path/to/file.tar}} {{image_name:tag1 image_name:tag2 ...}}`
