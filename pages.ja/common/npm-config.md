# npm config

> `npm` 構成設定を管理します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-config/>。

- すべての構成設定を表示します:

`npm {{[c|config]}} list`

- すべての構成設定を `JSON` としてリストします:

`npm {{[c|config]}} list --json`

- 特定の構成キーの値を取得します:

`npm {{[c|config]}} get {{key}}`

- 構成キーを特定の値に設定します:

`npm {{[c|config]}} set {{key}} {{value}}`

- 構成キーを削除します:

`npm {{[c|config]}} delete {{key}}`

- デフォルトのエディターで npm 構成ファイルを編集します (グローバル構成を編集するには、`--global` フラグを使用します):

`npm {{[c|config]}} edit`

- 無効な構成アイテムを修復してみます:

`npm {{[c|config]}} fix`
