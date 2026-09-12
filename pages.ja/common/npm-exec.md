# npm exec

> `npm` パッケージからバイナリを実行します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-exec/>。

- ローカルまたはリモートの `npm` パッケージからコマンドを実行します:

`npm {{[x|exec]}} {{command}} {{argument1 argument2 ...}}`

- パッケージを明示的に指定します (同じ名前のコマンドが複数存在する場合に便利です):

`npm {{[x|exec]}} --package {{package}} {{command}}`

- 現在のパスまたは `node_modules/.bin` にコマンドが存在する場合は、コマンドを実行します:

`npm {{[x|exec]}} --no-install {{command}} {{argument1 argument2 ...}}`

- 特定のコマンドを実行して、`npm` 自体からの出力を抑制します:

`npm {{[x|exec]}} --quiet {{command}} {{argument1 argument2 ...}}`

- ヘルプを表示する:

`npm {{[x|exec]}} --help`
