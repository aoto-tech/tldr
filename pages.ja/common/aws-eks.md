# aws eks

> Amazon Elastic Kubernetes Service (EKS) アドオン、クラスター、ノード グループを管理します。
> Amazon EKS は、AWS 上で Kubernetes を簡単に実行するためのサービスです。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/eks/>。

- EKS クラスターを作成します:

`aws eks create-cluster --name {{cluster_name}} --role-arn {{eks_service_role_arn}} --resources-vpc-config subnetIds={{subnet_ids}},securityGroupIds={{security_group_ids}}`

- EKS クラスターに接続するように kubeconfig を更新します:

`aws eks update-kubeconfig --name {{cluster_name}}`

- 利用可能な EKS クラスターをリストします:

`aws eks list-clusters`

- EKS クラスターの詳細を説明します:

`aws eks describe-cluster --name {{cluster_name}}`

- EKS クラスターを削除します:

`aws eks delete-cluster --name {{cluster_name}}`

- EKS クラスター内のノードグループを一覧表示します:

`aws eks list-nodegroups --cluster-name {{cluster_name}}`

- ノードグループの詳細を説明します:

`aws eks describe-nodegroup --cluster-name {{cluster_name}} --nodegroup-name {{nodegroup_name}}`
