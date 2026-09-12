# git reauthor

> 作成者IDの詳細を変更する。このコマンドはGit履歴を書き換えるため、次回のプッシュでは `--force` が必要になる。
> `git-extras` の一部。
> 詳細情報: <https://github.com/tj/git-extras/blob/main/Commands.md#git-reauthor>。

- Gitリポジトリ全体にわたって作成者のメールアドレスと名前を変更する:

`git reauthor {{[-o|--old-email]}} {{old@example.com}} {{[-e|--correct-email]}} {{new@example.com}} {{[-n|--correct-name]}} "{{名前}}"`

- メールアドレスと名前をGit設定で定義されたものに変更する:

`git reauthor {{[-o|--old-email]}} {{old@example.com}} {{[-c|--use-config]}}`

- 元の作成者にかかわらず、すべてのコミットのメールアドレスと名前を変更する:

`git reauthor {{[-a|--all]}} {{[-e|--correct-email]}} {{name@example.com}} {{[-n|--correct-name]}} {{名前}}`
