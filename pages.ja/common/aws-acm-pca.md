# aws acm-pca

> AWS Certificate Manager プライベート認証局。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/acm-pca/>。

- プライベート認証局を作成する:

`aws acm-pca create-certificate-authority --certificate-authority-configuration {{ca_config}} --idempotency-token {{token}} --permanent-deletion-time-in-days {{number}}`

- プライベート認証局の詳細を表示する:

`aws acm-pca describe-certificate-authority --certificate-authority-arn {{ca_arn}}`

- プライベート認証局を一覧表示する:

`aws acm-pca list-certificate-authorities`

- 認証局を更新する:

`aws acm-pca update-certificate-authority --certificate-authority-arn {{ca_arn}} --certificate-authority-configuration {{ca_config}} --status {{status}}`

- プライベート認証局を削除する:

`aws acm-pca delete-certificate-authority --certificate-authority-arn {{ca_arn}}`

- 証明書を発行する:

`aws acm-pca issue-certificate --certificate-authority-arn {{ca_arn}} --certificate-signing-request {{cert_signing_request}} --signing-algorithm {{algorithm}} --validity {{validity}}`

- 証明書を取り消する:

`aws acm-pca revoke-certificate --certificate-authority-arn {{ca_arn}} --certificate-serial {{serial}} --reason {{reason}}`

- 証明書の詳細を取得する:

`aws acm-pca get-certificate --certificate-authority-arn {{ca_arn}} --certificate-arn {{cert_arn}}`
