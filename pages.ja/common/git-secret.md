# git secret

> Gitリポジトリ内に非公開データを保存する。Bashで記述されている。
> 詳細情報: <https://github.com/sobolevn/git-secret>。

- ローカルリポジトリで `git-secret` を初期化する:

`git secret init`

- 現在のGitユーザーのメールアドレスにアクセスを許可する:

`git secret tell -m`

- メールアドレスを指定してアクセスを許可する:

`git secret tell {{メールアドレス}}`

- メールアドレスを指定してアクセスを取り消す:

`git secret killperson {{メールアドレス}}`

- シークレットへのアクセス権を持つメールアドレスを一覧表示する:

`git secret whoknows`

- シークレットファイルを登録する:

`git secret add {{ディレクトリ/サブディレクトリ/ファイル}}`

- シークレットを暗号化する:

`git secret hide`

- シークレットファイルを復号する:

`git secret reveal`
