# aws ssm

> AWS リソースと安全に対話し、管理する。
> 注: 対話型セッションでは、セッションマネージャープラグインがインストールされている必要がある。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/ssm/>。

- インスタンスでコマンドを実行する:

`aws ssm send-command --instance-ids {{instance_id1 instance_id2 ...}} --document-name "AWS-RunShellScript" --parameters 'commands=["{{command}}"]'`

- インスタンスでのコマンド呼び出しを確認する:

`aws ssm list-command-invocations --instance-id "{{instance_id}}"`

- 特定のコマンド呼び出しのコマンド出力を確認する:

`aws ssm list-command-invocations --command-id "{{command_id}}" --details`

- インスタンスとの対話型セッションを開始する:

`aws ssm start-session --target "{{instance_id}}"`

- リモートホストへのポート転送セッションを開始する:

`aws ssm start-session --target "{{instance_id}}" --document-name "AWS-StartPortForwardingSessionToRemoteHost" --parameters '{"portNumber":["{{remote_port}}"],"localPortNumber":["{{local_port}}"]}'`
