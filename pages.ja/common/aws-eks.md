# aws eks

> Amazon Elastic Kubernetes Service (EKS) アドオン、クラスター、ノードグループを管理する。
> Amazon EKS は、AWS 上で Kubernetes を簡単に実行するためのサービスである。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/eks/>。

- EKS クラスターを作成する:

`aws eks create-cluster --name {{cluster_name}} --role-arn {{eks_service_role_arn}} --resources-vpc-config subnetIds={{subnet_ids}},securityGroupIds={{security_group_ids}}`

- EKS クラスターに接続するように kubeconfig を更新する:

`aws eks update-kubeconfig --name {{cluster_name}}`

- 利用可能な EKS クラスターを一覧表示する:

`aws eks list-clusters`

- EKS クラスターの詳細の詳細を表示する:

`aws eks describe-cluster --name {{cluster_name}}`

- EKS クラスターを削除する:

`aws eks delete-cluster --name {{cluster_name}}`

- EKS クラスター内のノードグループを一覧表示する:

`aws eks list-nodegroups --cluster-name {{cluster_name}}`

- ノードグループの詳細の詳細を表示する:

`aws eks describe-nodegroup --cluster-name {{cluster_name}} --nodegroup-name {{nodegroup_name}}`
