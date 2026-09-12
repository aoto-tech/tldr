# aws accessanalyzer

> リソース ポリシーを分析およびレビューして、潜在的なセキュリティ リスクを特定します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/accessanalyzer/>。

- 新しいアクセス アナライザーを作成します:

`aws accessanalyzer create-analyzer --analyzer-name {{analyzer_name}} --type {{type}} --tags {{tags}}`

- 既存の Access Analyzer を削除します:

`aws accessanalyzer delete-analyzer --analyzer-arn {{analyzer_arn}}`

- 特定の Access Analyzer の詳細を取得します:

`aws accessanalyzer get-analyzer --analyzer-arn {{analyzer_arn}}`

- すべてのアクセス アナライザーをリストします:

`aws accessanalyzer list-analyzers`

- アクセス アナライザーの設定を更新します:

`aws accessanalyzer update-analyzer --analyzer-arn {{analyzer_arn}} --tags {{new_tags}}`

- 新しい Access Analyzer アーカイブ ルールを作成します:

`aws accessanalyzer create-archive-rule --analyzer-arn {{analyzer_arn}} --rule-name {{rule_name}} --filter {{filter}}`

- Access Analyzer のアーカイブ ルールを削除します:

`aws accessanalyzer delete-archive-rule --analyzer-arn {{analyzer_arn}} --rule-name {{rule_name}}`

- すべての Access Analyzer アーカイブ ルールをリストします:

`aws accessanalyzer list-archive-rules --analyzer-arn {{analyzer_arn}}`
