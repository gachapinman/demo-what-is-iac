# Terraform を使った IaC サンプル

1. 変数ファイルの作成

    `terraform.tfvars` ファイルに以下の変数を定義する

    | Name | Value |
    |---|---|
    |TENANT_ID  |テナントID|
    |SUBSCRIPTION_ID|サブスクリプションID|
    |location   |展開するリージョン（例：　`japaneast` ）|
    |prj        |プロジェクト名　（例： `xproject` ）|
    |env        |環境名 （例： `test` ）|
    |servername |サーバー名|
    |username   |サーバーのログインユーザー名|
    |password   |サーバーのログインパスワード|

    サンプルは以下の通り

    ```
    TENANT_ID       = "{YOUR-TENANT-ID}"
    SUBSCRIPTION_ID = "{YOUR-SUBSCRIPTION-ID}"
    location        = "japaneast"
    prj             = "at-terraform"
    env             = "test"
    servername      = "winsvr"
    username        = "azureuser"
    password        = "{YOUR-PASSOWRD}"
    ```

1. 以下の手順で展開

    1. 初期化

        ```
        terraform init
        ```

    1. Azureログイン

        ```
        az login
        az account set -s {YOUR-SUBSCRIPTION-ID}
        ```

    1. デプロイ

        ```
        terraform apply
        ```

