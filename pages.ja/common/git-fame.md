# git fame

> Gitリポジトリへの貢献を見やすく整形して出力する。
> 詳細情報: <https://manned.org/git-fame>。

- 現在のGitリポジトリへの貢献を計算する:

`git fame`

- 指定した正規表現に一致するファイルやディレクトリを除外する:

`git fame --excl "{{正規表現}}"`

- 指定した日付以降の貢献を計算する:

`git fame --since "{{3 weeks ago|2021-05-13}}"`

- 指定した形式で貢献を表示する:

`git fame --format {{pipe|yaml|json|csv|tsv}}`

- ファイル拡張子ごとの貢献を表示する:

`git fame {{[-t|--bytype]}}`

- 空白の変更を無視する:

`git fame {{[-w|--ignore-whitespace]}}`

- ファイル間で移動またはコピーされた行を検出する:

`git fame -C`

- ファイル内で移動またはコピーされた行を検出する:

`git fame -M`
