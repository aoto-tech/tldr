# systemctl isolate

> 指定したユニットとその依存関係を開始し、他のユニットをすべて停止します。
> `IgnoreOnIsolate=yes` を持つユニットを無視します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#isolate%20UNIT>。

- ターゲットに切り替えます (拡張子が指定されていない場合は、`.target` と想定されます):

`systemctl isolate {{target}}`

- グラフィカルターゲットに明示的に切り替えます:

`systemctl isolate graphical.target`

- レスキュー (シングルユーザー) モードに切り替えます:

`systemctl isolate rescue.target`

- 緊急モードに切り替えます:

`systemctl isolate emergency.target`
