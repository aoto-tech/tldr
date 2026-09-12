# npm sbom

> Node.js プロジェクトのソフトウェア部品表 (SBOM) を生成します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-sbom/>。

- プロジェクト内のすべての依存関係のリストを出力します:

`npm sbom`

- `dev` と `optional` の両方の依存関係を除外します:

`npm sbom --omit dev --omit optional`

- `package-lock.json` のみに基づいて SBOM を生成します:

`npm sbom --package-lock-only`
