# npm org

> 組織を管理します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-org/>。

- 新しいユーザーを組織に追加します:

`npm org set {{organization_name}} {{username}}`

- 組織内のユーザーの役割を変更します:

`npm org set {{organization_name}} {{username}} {{developer|admin|owner}}`

- 組織からユーザーを削除します:

`npm org rm {{organization_name}} {{username}}`

- 組織内のすべてのユーザーをリストします:

`npm org ls {{organization_name}}`

- 組織内のすべてのユーザーをリストし、JSON 形式で出力します:

`npm org ls {{organization_name}} --json`

- 組織内のユーザーの役割を表示します:

`npm org ls {{organization_name}} {{username}}`
