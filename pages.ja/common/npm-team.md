# npm team

> `npm` レジストリで組織内のチームを管理します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-team/>。

- 組織内のチームにユーザーを追加します:

`npm team add {{organization:team}} {{username}}`

- チームからユーザーを削除します:

`npm team rm {{organization:team}} {{username}}`

- 組織内に新しいチームを作成します:

`npm team create {{organization:team}}`

- 組織からチームを削除します:

`npm team destroy {{organization:team}}`

- 組織内のすべてのチームをリストします:

`npm team ls {{organization}}`

- 特定のチーム内のすべてのユーザーをリストします:

`npm team ls {{organization:team}}`
