# systemctl kexec

> kexec 経由でシステムを再起動します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#kexec>。

- kexec を使用した高速リブート (カーネルがプリロードされている場合):

`systemctl kexec`

- kexec が利用可能な場合でも、通常の再起動を強制します:

`systemctl kexec {{[-f|--force]}}`
