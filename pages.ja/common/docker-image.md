# docker image

> Docker イメージを管理します。
> 「`docker build`」、「`docker image pull`」、「`docker image rm`」も参照してください。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/image/>。

- ローカルの Docker イメージをリストします:

`docker {{[images|image ls]}}`

- 未使用のローカル Docker イメージを削除します:

`docker image prune`

- 未使用のイメージをすべて削除します (タグのないイメージだけでなく):

`docker image prune {{[-a|--all]}}`

- ローカルの Docker イメージの履歴を表示します:

`docker {{[history|image history]}} {{image}}`
