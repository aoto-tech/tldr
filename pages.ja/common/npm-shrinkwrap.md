# npm shrinkwrap

> パッケージの依存関係をロックダウンし、`npm-shrinkwrap.json` ファイルを作成します。
> `package-lock.json` に似ていますが、公開されたパッケージを対象としています。
> 詳細情報: <https://docs.npmjs.com/cli/v11/npm-shrinkwrap>。

- 現在の `package-lock.json` から `npm-shrinkwrap.json` ファイルを生成します:

`npm shrinkwrap`

- 運用モードで実行します (devDependency を除く):

`npm shrinkwrap --production`

- シュリンクラップ ファイルが既に存在する場合でも、強制的に再作成します:

`npm shrinkwrap --force`
