# git magic

> Gitのadd、commit、pushの一連の操作を自動化する。
> `git-extras` の一部。
> 詳細情報: <https://manned.org/git-magic>。

- 自動生成したメッセージで変更をコミットする:

`git magic`

- 追跡されていないファイルを[a]ddし、自動生成したメッセージで変更をコミットする:

`git magic -a`

- 独自の[m]essageで変更をコミットする:

`git magic -m "{{コミットメッセージ}}"`

- コミット前にコミット[m]essageを[e]ditする:

`git magic -em "{{コミットメッセージ}}"`

- 変更をコミットしてリモートへ[p]ushする:

`git magic -p`

- 変更をコミットし、リモートへ[f]orce [p]ushする:

`git magic -fp`
