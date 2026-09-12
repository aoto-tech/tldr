# git-lfs-transfer

> Git LFSの純粋なSSH転送プロトコルをサーバー側で実装する。
> Git LFSがHTTPSの代わりにSSH経由で大容量ファイルをアップロード、ダウンロードできるようにする。
> 詳細情報: <https://github.com/charmbracelet/git-lfs-transfer#usage>。

- Git LFSで追跡している大容量ファイルをリポジトリへアップロードする:

`git-lfs-transfer {{repo.gitへのパス}} upload`

- Git LFSで追跡している大容量ファイルをリポジトリからダウンロードする:

`git-lfs-transfer {{repo.gitへのパス}} download`
