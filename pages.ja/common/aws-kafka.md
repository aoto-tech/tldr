# aws kafka

> Amazon Managed Streaming for Apache Kafka (Amazon MSK) クラスターを管理する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/kafka/>。

- 新しい MSK クラスターを作成する:

`aws kafka create-cluster --cluster-name {{cluster_name}} --broker-node-group-info instanceType={{instance_type}},clientSubnets={{subnet_id1 subnet_id2 ...}} --kafka-version {{version}} --number-of-broker-nodes {{number}}`

- MSK クラスターの詳細を表示する:

`aws kafka describe-cluster --cluster-arn {{cluster_arn}}`

- 現在のリージョン内のすべての MSK クラスターを一覧表示する:

`aws kafka list-clusters`

- 新しい MSK 設定を作成する:

`aws kafka create-configuration --name {{configuration_name}} --server-properties file://{{path/to/configuration_file.txt}}`

- MSK 設定の詳細を表示する:

`aws kafka describe-configuration --arn {{configuration_arn}}`

- 現在のリージョン内のすべての MSK 設定を一覧表示する:

`aws kafka list-configurations`

- MSK クラスター設定を更新する:

`aws kafka update-cluster-configuration --cluster-arn {{cluster_arn}} --configuration-info arn={{configuration_arn}},revision={{configuration_revision}}`

- MSK クラスターを削除する:

`aws kafka delete-cluster --cluster-arn {{cluster_arn}}`
