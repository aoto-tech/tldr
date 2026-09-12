# aws ses

> AWS Simple Email Service の CLI。
> 大規模な受信および送信クラウド電子メール サービス。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/ses/>。

- 新しい受信ルール セットを作成します:

`aws ses create-receipt-rule-set --rule-set-name {{rule_set_name}} --generate-cli-skeleton`

- アクティブな受信ルール セットについて説明します:

`aws ses describe-active-receipt-rule-set --generate-cli-skeleton`

- 特定の受信ルールを説明します:

`aws ses describe-receipt-rule --rule-set-name {{rule_set_name}} --rule-name {{rule_name}} --generate-cli-skeleton`

- すべての受信ルール セットをリストします:

`aws ses list-receipt-rule-sets --starting-token {{token_string}} --max-items {{integer}} --generate-cli-skeleton`

- 特定の受信ルール セットを削除します (現在アクティブなルール セットは削除できません):

`aws ses delete-receipt-rule-set --rule-set-name {{rule_set_name}} --generate-cli-skeleton`

- 特定の受信ルールを削除します:

`aws ses delete-receipt-rule --rule-set-name {{rule_set_name}} --rule-name {{rule_name}} --generate-cli-skeleton`

- 電子メールを送信します:

`aws ses send-email --from {{from_address}} --destination "ToAddresses={{addresses}}" --message "Subject={Data={{subject_text}},Charset=utf8},Body={Text={Data={{body_text}},Charset=utf8},Html={Data={{message_body_containing_html}},Charset=utf8\}\}"`

- 特定の SES サブコマンドのヘルプを表示します:

`aws ses {{subcommand}} help`
