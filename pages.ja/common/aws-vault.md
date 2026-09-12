# aws-vault

> 開発環境で AWS 認証情報を安全に保存し、アクセスするためのボールト。
> 詳細情報: <https://github.com/99designs/aws-vault>。

- 認証情報を安全なキーストアに追加します:

`aws-vault add {{profile}}`

- 環境内で AWS 認証情報を使用してコマンドを実行します:

`aws-vault exec {{profile}} -- {{aws s3 ls}}`

- ブラウザウィンドウを開いて、AWS コンソールにログインします:

`aws-vault login {{profile}}`

- プロファイルとその認証情報およびセッションを一覧表示します:

`aws-vault list`

- AWS 認証情報をローテーションします:

`aws-vault rotate {{profile}}`

- 安全なキーストアから認証情報を削除します:

`aws-vault remove {{profile}}`
