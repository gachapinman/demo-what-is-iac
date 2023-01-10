# ARM Template を使った IaC サンプル

1. 以下のボタンを押下

    [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fakinaritsugo%2Fdemo-what-is-iac%2Fmain%2Farm%2Ftemplate.json)

1. 以下の項目を入力

    | Name | Value |
    |---|---|
    |サブスクリプション  |利用したいサブスクリプション|
    |リソースグループ    |展開したい先のリソースグループ名|
    |リージョン          |展開するリージョン（例：　`Japan East` ）|
    |Prj                |プロジェクト名　（例： `xproject` ）|
    |Env                |環境名 （例： `test` ）|
    |Servername         |サーバー名|
    |Username           |サーバーのログインユーザー名|
    |Password           |サーバーのログインパスワード|

1. 「確認と作成」を選択

1. 「作成」を選択

1. Azureへリソースが展開されたことを確認
