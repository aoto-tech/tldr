# aws codeartifact

> CodeArtifact リポジトリ、ドメイン、パッケージ、パッケージバージョン、およびアセットを管理する。
> CodeArtifact は、Maven、Gradle、npm、Yarn、Twine、pip、NuGet、SwiftPM などの一般的なパッケージマネージャーやビルドツールと互換性のあるアーティファクトリポジトリである。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/codeartifact/>。

- AWS アカウントで利用可能なドメインを一覧表示する:

`aws codeartifact list-domains`

- 特定のパッケージマネージャーの資格情報を生成する:

`aws codeartifact login --tool {{npm|pip|twine}} --domain {{your_domain}} --repository {{repository_name}}`

- CodeArtifact リポジトリのエンドポイント URL を取得する:

`aws codeartifact get-repository-endpoint --domain {{your_domain}} --repository {{repository_name}} --format {{npm|pypi|maven|nuget|generic}}`

- ヘルプを表示する:

`aws codeartifact help`

- 特定のサブコマンドのヘルプを表示する:

`aws codeartifact {{subcommand}} help`
