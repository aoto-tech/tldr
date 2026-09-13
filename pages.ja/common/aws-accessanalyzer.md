# aws accessanalyzer

> リソースポリシーを分析およびレビューして、潜在的なセキュリティリスクを特定する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/accessanalyzer/>。

- 新しいアクセスアナライザーを作成する:

`aws accessanalyzer create-analyzer --analyzer-name {{analyzer_name}} --type {{type}} --tags {{tags}}`

- 既存の Access Analyzer を削除する:

`aws accessanalyzer delete-analyzer --analyzer-arn {{analyzer_arn}}`

- 特定の Access Analyzer の詳細を取得する:

`aws accessanalyzer get-analyzer --analyzer-arn {{analyzer_arn}}`

- すべてのアクセスアナライザーを一覧表示する:

`aws accessanalyzer list-analyzers`

- アクセスアナライザーの設定を更新する:

`aws accessanalyzer update-analyzer --analyzer-arn {{analyzer_arn}} --tags {{new_tags}}`

- 新しい Access Analyzer アーカイブルールを作成する:

`aws accessanalyzer create-archive-rule --analyzer-arn {{analyzer_arn}} --rule-name {{rule_name}} --filter {{filter}}`

- Access Analyzer のアーカイブルールを削除する:

`aws accessanalyzer delete-archive-rule --analyzer-arn {{analyzer_arn}} --rule-name {{rule_name}}`

- すべての Access Analyzer アーカイブルールを一覧表示する:

`aws accessanalyzer list-archive-rules --analyzer-arn {{analyzer_arn}}`
