# aws-vault

> 開発環境で AWS 認証情報を安全に保存し、アクセスするためのボールト。
> 詳細情報: <https://github.com/99designs/aws-vault>。

- 認証情報を安全なキーストアに追加する:

`aws-vault add {{profile}}`

- 環境内で AWS 認証情報を使用してコマンドを実行する:

`aws-vault exec {{profile}} -- {{aws s3 ls}}`

- ブラウザウィンドウを開いて、AWS コンソールにログインする:

`aws-vault login {{profile}}`

- プロファイルとその認証情報およびセッションを一覧表示する:

`aws-vault list`

- AWS 認証情報をローテーションする:

`aws-vault rotate {{profile}}`

- 安全なキーストアから認証情報を削除する:

`aws-vault remove {{profile}}`
