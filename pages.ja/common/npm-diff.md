# npm diff

> `npm` レジストリからパッケージのバージョンを比較し、違いを示します。
> `git diff` に似ています。
> 詳細情報: <https://docs.npmjs.com/cli/npm-diff/>。

- 2 つの特定のパッケージ バージョンを比較します:

`npm diff --diff {{package_name}}@{{version1}} --diff {{package_name}}@{{version2}}`

- 現在のローカル パッケージと最新の公開バージョンを比較します:

`npm diff`

- 現在のローカル パッケージを特定のバージョンと比較します:

`npm diff --diff {{package_name}}@{{version}}`

- 現在のディレクトリ内のパッケージとレジストリのバージョンを比較します:

`npm diff --diff {{package_name}}`

- 異なるファイル名のみを表示します:

`npm diff --diff-name-only --diff {{package_name}}@{{version1}} --diff {{package_name}}@{{version2}}`

- 特定のファイルまたはディレクトリのみを比較します:

`npm diff {{path/to/file_or_directory}} --diff {{package_name}}@{{version1}} --diff {{package_name}}@{{version2}}`

- 比較するときに空白を無視します:

`npm diff --diff-ignore-all-space --diff {{package_name}}@{{version1}} --diff {{package_name}}@{{version2}}`
