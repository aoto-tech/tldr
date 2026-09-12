# docker login

> Docker レジストリにログインします。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/login/>。

- レジストリに対話的にログインします:

`docker login`

- 特定のユーザー名でレジストリにログインします (ユーザーはパスワードの入力を求められます):

`docker login {{[-u|--username]}} {{username}}`

- ユーザー名とパスワードを使用してレジストリにログインします:

`docker login {{[-u|--username]}} {{username}} {{[-p|--password]}} {{password}} {{server}}`

- `stdin` のパスワードを使用してレジストリにログインします:

`echo "{{password}}" | docker login {{[-u|--username]}} {{username}} --password-stdin`
