# npm audit

> プロジェクトの依存関係をスキャンして、既知のセキュリティ脆弱性を探します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-audit/>。

- プロジェクトの依存関係をスキャンして既知の脆弱性を探します:

`npm audit`

- プロジェクトの依存関係の脆弱性を自動的に修正します:

`npm audit fix`

- 脆弱性のある依存関係を強制的に自動修正します:

`npm audit fix {{[-f|--force]}}`

- `node_modules` ディレクトリを変更せずにロック ファイルを更新します:

`npm audit fix --package-lock-only`

- 変更を加えずに修正プロセスをシミュレートします:

`npm audit fix --dry-run`

- 監査結果を JSON 形式で出力します:

`npm audit --json`

- 指定された重大度を超える脆弱性のみで監査が失敗するように監査を構成します:

`npm audit --audit-level {{info|low|moderate|high|critical}}`
