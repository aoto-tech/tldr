# aws workmail

> Amazon WorkMail を管理します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/workmail/>。

- すべての WorkMail 組織を一覧表示する:

`aws workmail list-organizations`

- 指定した組織のすべてのユーザーを一覧表示する:

`aws workmail list-users --organization-id {{organization_id}}`

- 指定した組織に WorkMail ユーザーを作成する:

`aws workmail create-user --name {{username}} --display-name {{name}} --password {{password}} --organization-id {{organization_id}}`

- グループまたはユーザーを WorkMail に登録して有効化する:

`aws workmail register-to-work-mail --entity-id {{entity_id}} --email {{email}} --organization-id {{organization_id}}`

- 指定した組織に WorkMail グループを作成する:

`aws workmail create-group --name {{group_name}} --organization-id {{organization_id}}`

- 指定したグループにメンバーを関連付ける:

`aws workmail associate-member-to-group --group-id {{group_id}} --member-id {{member_id}} --organization-id {{organization_id}}`

- WorkMail からユーザーまたはグループの登録を解除して無効化する:

`aws workmail deregister-from-work-mail --entity-id {{entity_id}} --organization-id {{organization_id}}`

- 組織からユーザーを削除する:

`aws workmail delete-user --user-id {{user_id}} --organization-id {{organization_id}}`
