# npm deprecate

> `npm` パッケージのバージョンまたはバージョンの範囲を非推奨としてマークします。
> 詳細情報: <https://docs.npmjs.com/cli/npm-deprecate/>。

- パッケージの特定のバージョンを非推奨にします:

`npm deprecate {{package_name}}@{{version}} "{{deprecation_message}}"`

- パッケージのさまざまなバージョンを非推奨にします:

`npm deprecate {{package_name}}@"<{{version_range}}" "{{deprecation_message}}"`

- パッケージの特定のバージョンの非推奨を解除します:

`npm deprecate {{package_name}}@{{version}} ""`
