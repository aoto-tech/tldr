# jj config set

> 構成オプションを特定の値に設定します。
> 値は TOML 式として指定されます。
> `jj config unset` も参照してください。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-config-set>。

- ユーザーレベルの設定でユーザー名を設定します:

`jj config {{[s|set]}} --user user.name "{{name}}"`

- ユーザーレベルの構成でユーザーの電子メールを設定します:

`jj config {{[s|set]}} --user user.email "{{email}}"`

- リポジトリレベルの構成で構成オプションを設定します:

`jj config {{[s|set]}} --repo {{name}} {{value}}`

- ワークスペースレベルの構成で構成オプションを設定します:

`jj config {{[s|set]}} --workspace {{name}} {{value}}`

- ブール値の構成オプションを設定します:

`jj config {{[s|set]}} --user {{name}} {{true|false}}`
