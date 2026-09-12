# aws kafka

> Amazon MSK (マネージド ストリーミング for Apache Kafka) クラスターを管理します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/kafka/>。

- 新しい MSK クラスターを作成します:

`aws kafka create-cluster --cluster-name {{cluster_name}} --broker-node-group-info instanceType={{instance_type}},clientSubnets={{subnet_id1 subnet_id2 ...}} --kafka-version {{version}} --number-of-broker-nodes {{number}}`

- MSK クラスターについて説明します:

`aws kafka describe-cluster --cluster-arn {{cluster_arn}}`

- 現在のリージョン内のすべての MSK クラスターを一覧表示します:

`aws kafka list-clusters`

- 新しい MSK 構成を作成します:

`aws kafka create-configuration --name {{configuration_name}} --server-properties file://{{path/to/configuration_file.txt}}`

- MSK 構成について説明します:

`aws kafka describe-configuration --arn {{configuration_arn}}`

- 現在のリージョン内のすべての MSK 構成をリストします:

`aws kafka list-configurations`

- MSK クラスター構成を更新します:

`aws kafka update-cluster-configuration --cluster-arn {{cluster_arn}} --configuration-info arn={{configuration_arn}},revision={{configuration_revision}}`

- MSK クラスターを削除します:

`aws kafka delete-cluster --cluster-arn {{cluster_arn}}`
