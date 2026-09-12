# git paste

> `pastebinit` を使用してコミットをPastebinサイトへ送信する。
> `git-extras` の一部。
> 詳細情報: <https://github.com/tj/git-extras/blob/main/Commands.md#git-paste>。

- 現在のブランチと上流ブランチ間のパッチを、`pastebinit` を使用してPastebinへ送信する:

`git paste`

- 別のコミット範囲を選択するため、オプションを `git format-patch` へ渡す (`@^` は `HEAD` の親を選択するため、現在チェックアウトしているコミットが送信される):

`git paste {{@^}}`
