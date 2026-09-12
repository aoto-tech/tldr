# npm install

> ノード パッケージをインストールします。
> 詳細情報: <https://docs.npmjs.com/cli/npm-install/>。

- `package.json` にリストされている依存関係をインストールします:

`npm {{[i|install]}}`

- 特定のバージョンのパッケージをダウンロードし、`package.json` の依存関係のリストに追加します:

`npm {{[i|install]}} {{package_name}}@{{version}}`

- パッケージの最新バージョンをダウンロードし、`package.json` の開発依存関係のリストに追加します:

`npm {{[i|install]}} {{package_name}} {{[-D|--save-dev]}}`

- パッケージの最新バージョンをダウンロードし、グローバルにインストールします (`npm config set prefix` でインストール場所を設定します):

`npm {{[i|install]}} {{package_name}} {{[-g|--global]}}`
