# npm explain

> パッケージのインストール方法を説明し、その依存関係と含める理由を詳しく説明します。
> 詳細情報: <https://docs.npmjs.com/cli/explain/>。

- 特定のパッケージがインストールされる理由を説明します:

`npm {{[why|explain]}} {{package_name}}`

- 説明を JSON 形式で表示します:

`npm {{[why|explain]}} {{package_name}} --json`

- 説明にピアの依存関係を含めます:

`npm {{[why|explain]}} {{package_name}} --include peer`

- 説明の深さを 2 レベルの深さに制限します:

`npm {{[why|explain]}} {{package_name}} --depth 2`
