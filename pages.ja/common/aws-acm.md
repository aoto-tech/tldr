# aws acm

> AWS 証明書マネージャー。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/acm/>。

- 証明書をインポートします:

`aws acm import-certificate --certificate-arn {{certificate_arn}} --certificate {{certificate}} --private-key {{private_key}} --certificate-chain {{certificate_chain}}`

- 証明書をリストします:

`aws acm list-certificates`

- 証明書について説明します:

`aws acm describe-certificate --certificate-arn {{certificate_arn}}`

- 証明書を要求します:

`aws acm request-certificate --domain-name {{domain_name}} --validation-method {{validation_method}}`

- 証明書を削除します:

`aws acm delete-certificate --certificate-arn {{certificate_arn}}`

- 証明書の検証をリストします:

`aws acm list-certificates --certificate-statuses {{status}}`

- 証明書の詳細を取得します:

`aws acm get-certificate --certificate-arn {{certificate_arn}}`

- 証明書オプションを更新します:

`aws acm update-certificate-options --certificate-arn {{certificate_arn}} --options {{options}}`
