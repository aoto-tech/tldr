# git show

> さまざまな種類の Git オブジェクト (コミット、タグなど) を表示する。
> 詳細情報: <https://git-scm.com/docs/git-show>。

- 最新コミットの情報 (ハッシュ、メッセージ、変更内容、その他のメタデータ) を表示する:

`git show`

- 指定したコミット、タグ、ブランチ (`HEAD` など) の情報を表示する:

`git show {{commit|tag|branch}}`

- 追加、リネーム、削除されたファイルの一覧だけを表示する:

`git show --summary {{commit}}`

- 行の比較時に空白を無視する:

`git show {{[-w|--ignore-all-space]}}`

- 差分出力を抑制し、コミットメッセージを1行で表示する:

`git show --oneline {{[-s|--no-patch]}} {{commit}}`

- 変更されたファイルの差分統計 (追加行数や削除行数など) を表示する:

`git show --stat {{commit}}`

- コミットで変更されたすべてのファイル (変更、追加、削除) の簡略一覧を表示する:

`git show --name-only {{commit}}`

- 指定したリビジョン (ブランチ、タグ、コミットなど) 時点のファイル内容を表示する:

`git show {{revision}}:{{path/to/file}}`
