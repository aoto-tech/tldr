# aws codeartifact

> CodeArtifact リポジトリ、ドメイン、パッケージ、パッケージ バージョン、およびアセットを管理します。
> CodeArtifact は、Maven、Gradle、npm、Yarn、Twine、pip、NuGet、SwiftPM などの一般的なパッケージ マネージャーやビルド ツールと互換性のあるアーティファクト リポジトリです。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/codeartifact/>。

- AWS アカウントで利用可能なドメインをリストします:

`aws codeartifact list-domains`

- 特定のパッケージ マネージャーの資格情報を生成します:

`aws codeartifact login --tool {{npm|pip|twine}} --domain {{your_domain}} --repository {{repository_name}}`

- CodeArtifact リポジトリのエンドポイント URL を取得します:

`aws codeartifact get-repository-endpoint --domain {{your_domain}} --repository {{repository_name}} --format {{npm|pypi|maven|nuget|generic}}`

- ヘルプを表示する:

`aws codeartifact help`

- 特定のサブコマンドのヘルプを表示します:

`aws codeartifact {{subcommand}} help`
