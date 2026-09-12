# npm install-test

> `npm install` の後に `npm test` を実行するのと同じです。
> 注: `it` は、`install-test` の短縮形として使用できます。
> 詳細情報: <https://docs.npmjs.com/cli/npm-install-test/>。

- すべての依存関係をインストールしてから、テストを実行します:

`npm {{[it|install-test]}}`

- 特定のパッケージをインストールしてテストを実行します:

`npm {{[it|install-test]}} {{package_name}}`

- パッケージをインストールし、テストを実行する前に依存関係として保存します:

`npm {{[it|install-test]}} {{package_name}} {{[-S|--save]}}`

- 依存関係をグローバルにインストールし、テストを実行します:

`npm {{[it|install-test]}} {{[-g|--global]}}`
