# git standup

> 指定したユーザーのコミットを表示する。
> `git-extras` の一部。
> 詳細情報: <https://manned.org/git-standup>。

- 指定した作成者による過去10日間のコミットを表示する:

`git standup -a {{名前|メールアドレス}} -d 10`

- 指定した作成者による過去10日間のコミットと、GPG署名の有無を表示する:

`git standup -a {{名前|メールアドレス}} -d 10 -g`

- すべての貢献者による過去10日間のすべてのコミットを表示する:

`git standup -a all -d 10`

- ヘルプを表示する:

`git standup -h`
