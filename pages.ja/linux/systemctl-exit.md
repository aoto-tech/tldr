# systemctl exit

> サービスマネージャーに終了するように依頼してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#exit%20EXIT_CODE>。

- ユーザー サービス マネージャーを終了します:

`systemctl exit --user`

- 特定の終了コードを使用してユーザー サービス マネージャーを終了します:

`systemctl exit {{code}} --user`

- コンテナのサービス マネージャーに終了を依頼します (コンテナ内にない場合は、`systemctl poweroff` に相当します):

`systemctl exit`
