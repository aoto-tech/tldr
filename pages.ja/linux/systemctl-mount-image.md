# systemctl mount-image

> イメージ ファイルをユニットのマウント名前空間にマウントします。
> マウントスペース内で実行されるユニット (`RootImage=`、`PrivateMounts=` など) でのみサポートされます。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#mount-image%20UNIT%20IMAGE%20%5BPATH%20%5BPARTITION_NAME:MOUNT_OPTIONS%5D%5D>。

- ユニットのマウント名前空間内の特定のパスにイメージをマウントします:

`systemctl mount-image {{unit}} /{{path/to/image}} /{{path/to/directory_inside_unit}}`

- イメージの `root` パーティションを読み取り専用および no-setuid オプションでマウントします:

`systemctl mount-image {{unit}} /{{path/to/image}} /{{path/to/directory_inside_unit}} root:ro,nosuid`

- マウントする前に宛先ディレクトリを作成します:

`systemctl mount-image --mkdir {{unit}} /{{path/to/image}} /{{path/to/directory_inside_unit}}`

- イメージを読み取り専用としてマウントします:

`systemctl mount-image --read-only {{unit}} /{{path/to/image}} /{{path/to/directory_inside_unit}}`
