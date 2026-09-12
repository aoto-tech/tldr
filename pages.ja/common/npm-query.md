# npm query

> CSS のようなセレクターを使用して、依存関係オブジェクトの配列を出力します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-query/>。

- 直接の依存関係を出力します:

`npm query ':root > *'`

- すべての直接の運用/開発依存関係を出力します:

`npm query ':root > .{{prod|dev}}'`

- 依存関係を特定の名前で出力します:

`npm query '#{{package}}'`

- 特定の名前とセマンティック バージョン管理範囲内の依存関係を出力します:

`npm query '#{{package}}@{{semantic_version}}'`

- 依存関係のない依存関係を出力します:

`npm query ':empty'`

- ポストインストール スクリプトを使用してすべての依存関係を検索し、アンインストールします:

`npm query ":attr(scripts, [postinstall])" | jq 'map(.name) | join("\n")' {{[-r|--raw-output]}} | xargs -I _ npm uninstall _`

- すべての Git 依存関係を検索し、どのアプリケーションがそれらを必要とするかを出力します:

`npm query ":type(git)" | jq 'map(.name)' | xargs -I _ npm why _`
