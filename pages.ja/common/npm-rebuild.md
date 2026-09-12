# npm rebuild

> ノードまたは依存関係の変更後にネイティブ Node.js パッケージを再構築します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-rebuild/>。

- 特定のパッケージを再構築します:

`npm {{[rb|rebuild]}} {{package}}`

- インストールされているすべてのパッケージを再構築します:

`npm {{[rb|rebuild]}}`

- 詳細な出力を使用して再構築します:

`npm {{[rb|rebuild]}} --verbose`

- 特定のディレクトリでパッケージを再構築します:

`npm {{[rb|rebuild]}} --prefix {{path/to/dir}} {{package}}`

- npm キャッシュを使用せずに再構築します:

`npm {{[rb|rebuild]}} --no-cache`

- グローバル モードで再構築します:

`npm {{[rb|rebuild]}} {{[-g|--global]}}`
