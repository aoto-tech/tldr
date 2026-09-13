# aws-google-auth

> Google Apps をフェデレーション (シングル サインオン) プロバイダーとして使用して、AWS 一時 (STS) 認証情報を取得します。
> 詳細情報: <https://github.com/cevoaustralia/aws-google-auth>。

- 指定したユーザー名 IDP および SP 識別子を使用して Google SSO でログインし、認証情報の有効期間を 1 時間に設定します:

`aws-google-auth {{[-u|--username]}} {{example@example.com}} {{[-I|--idp-id]}} {{$GOOGLE_IDP_ID}} {{[-S|--sp-id]}} {{$GOOGLE_SP_ID}} {{[-d|--duration]}} {{3600}}`

- ログインして、どのロールを使用するかを尋ねます (利用可能な SAML ロールが複数ある場合):

`aws-google-auth {{[-u|--username]}} {{example@example.com}} {{[-I|--idp-id]}} {{$GOOGLE_IDP_ID}} {{[-S|--sp-id]}} {{$GOOGLE_SP_ID}} {{[-d|--duration]}} {{3600}} {{[-a|--ask-role]}}`

- AWS アカウントのエイリアスを解決します:

`aws-google-auth {{[-u|--username]}} {{example@example.com}} {{[-I|--idp-id]}} {{$GOOGLE_IDP_ID}} {{[-S|--sp-id]}} {{$GOOGLE_SP_ID}} {{[-d|--duration]}} {{3600}} {{[-a|--ask-role]}} --resolve-aliases`

- ヘルプを表示する:

`aws-google-auth {{[-h|--help]}}`
