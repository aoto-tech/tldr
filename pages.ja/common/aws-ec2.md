# aws ec2

> AWS EC2 インスタンスとボリュームを管理します。
> AWS EC2 は、アプリケーションの開発とデプロイを迅速化するために、AWS クラウド内に安全でサイズ変更可能なコンピューティング容量を提供します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/ec2/>。

- 特定のインスタンスに関する情報を表示します:

`aws ec2 describe-instances --instance-ids {{instance_id}}`

- すべてのインスタンスに関する情報を表示します:

`aws ec2 describe-instances`

- すべての EC2 ボリュームに関する情報を表示します:

`aws ec2 describe-volumes`

- EC2 ボリュームを削除します:

`aws ec2 delete-volume --volume-id {{volume_id}}`

- EC2 ボリュームからスナップショットを作成します:

`aws ec2 create-snapshot --volume-id {{volume_id}}`

- 利用可能な AMI (Amazon マシン イメージ) をリストします:

`aws ec2 describe-images`

- 使用可能なすべての EC2 コマンドのリストを表示します:

`aws ec2 help`

- 特定の EC2 サブコマンドのヘルプを表示します:

`aws ec2 {{subcommand}} help`
