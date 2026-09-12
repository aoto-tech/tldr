# systemctl import-environment

> 環境変数をシェルから systemd の環境にインポートします。
> 「`systemctl show-environment`」、「`systemctl unset-environment`」も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#import-environment%20VARIABLE%E2%80%A6>。

- 変数をインポートします:

`systemctl import-environment {{variable}}`

- 複数の変数をインポートします:

`systemctl import-environment {{variable_1 variable_2 ...}}`

- ユーザー サービスの変数をインポートします:

`systemctl import-environment {{variable}} --user`
