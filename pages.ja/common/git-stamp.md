# git stamp

> バグトラッカーの問題番号やレビューページへのリンクを参照できるよう、直前のコミットメッセージに印を付ける。
> `git-extras` の一部。
> 詳細情報: <https://manned.org/git-stamp>。

- バグトラッカーの問題番号を参照する印を直前のコミットメッセージに付ける:

`git stamp {{問題番号}}`

- レビューページへリンクする印を直前のコミットメッセージに付ける:

`git stamp {{Review https://example.org/path/to/review}}`

- 以前の問題番号を新しい番号に置き換えて、直前のコミットメッセージに印を付ける:

`git stamp {{[-r|--replace]}} {{問題番号}}`
