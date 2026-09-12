# npm unpublish

> npm レジストリからパッケージを削除します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-unpublish/>。

- 特定のパッケージ バージョンを非公開にします:

`npm unpublish {{package_name}}@{{version}}`

- パッケージ全体を非公開にします:

`npm unpublish {{package_name}} {{[-f|--force]}}`

- スコープが設定されているパッケージを非公開にします:

`npm unpublish @{{scope}}/{{package_name}}`

- 非公開にするまでのタイムアウト期間を指定します:

`npm unpublish {{package_name}} --timeout {{time_in_milliseconds}}`

- 実際に実行せずに何が非公開になるかを確認するためのドライラン:

`npm unpublish {{package_name}} --dry-run`
