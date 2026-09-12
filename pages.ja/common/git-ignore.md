# git ignore

> `.gitignore` ファイルを表示、更新する。
> `git-extras` の一部。
> 参照: `git ignore-io`。
> 詳細情報: <https://github.com/tj/git-extras/blob/main/Commands.md#git-ignore>。

- グローバルとローカルのすべての `.gitignore` ファイルの内容を表示する:

`git ignore`

- `.git/info/exclude` ファイルを更新し、ファイルを非公開で無視する:

`git ignore {{ファイルパターン}} {{[-p|--private]}}`

- ローカルの `.gitignore` ファイルを更新し、ファイルをローカルで無視する:

`git ignore {{ファイルパターン}}`

- グローバルの `.gitignore` ファイルを更新し、ファイルをグローバルで無視する:

`git ignore {{ファイルパターン}} {{[-g|--global]}}`
