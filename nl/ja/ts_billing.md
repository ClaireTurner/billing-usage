---

copyright:
  years: 2017, 2019
lastupdated: "2019-06-11"

keywords: troubleshoot billing, billing error, payment error, error message, feature code, subscription code

subcollection: billing-usage

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:tsSymptoms: .tsSymptoms}
{:tsCauses: .tsCauses}
{:tsResolve: .tsResolve}
{:troubleshoot: data-hd-content-type='troubleshoot'}


# 請求および使用量の管理に関するトラブルシューティング
{: #troubleshoot}

請求および使用量の管理の一般的な問題には、請求処理情報にアクセスするために必要な権限が含まれる場合があります。 多くの場合、いくつかの簡単なステップに従うことで、この問題から復旧できます。
{:shortdesc}


## 請求処理情報にアクセスできないのはなぜですか?
{: #cannot-access-billing-info}
{: troubleshoot}

支払いや送り状などの請求処理情報にアクセスしようとすると、機能が使用できないことを示すメッセージが表示されます。
{: tsSymptoms}

このメッセージを受け取る理由は、ユーザーがアカウントの請求処理情報を表示する権限を持っていないためです。 アカウント所有者か Cloud Foundry 組織請求マネージャーであるか、または管理者役割が割り当てられているすべてのアカウント管理サービスで IAM ポリシーを持っている必要があります。
{: tsCauses}

アカウント所有者であれば、そのアカウントの請求処理情報を表示できます。 請求管理者は、Cloud Foundry 組織の請求処理情報を表示できます。 また、IAM 対応リソースの場合は、管理者役割が割り当てられているすべてのアカウント管理サービスに対して IAM ポリシーが必要です。

以下のステップを実行してアクセス権限を確認します。

  1. **「管理」 > 「アクセス (IAM)」**に移動して、**「ユーザー」**を選択します。
  2. 「ユーザー」ページから自分の名前をクリックします。
  3. **「アクセス・ポリシー」**をクリックして、割り当てられている IAM アクセス・ポリシーを表示します。
  4. **「Cloud Foundry アクセス権限」**をクリックし、割り当てられた組織の行を展開して、アカウント所有者または請求管理者の役割を持っているかどうかを確認します。

IAM アクセス権限について詳しくは、[Cloud IAM 役割](/docs/iam?topic=iam-userroles)を参照してください。 Cloud Foundry アクセス権限について詳しくは、[Cloud Foundry の役割](/docs/iam?topic=iam-cfaccess)を参照してください。
{: tsResolve}


## フィーチャー・コードを適用できないのはなぜですか?
{: #cannot-apply-feature-code}
{: troubleshoot}

フィーチャー・コードを適用しようとしたときに、そのコードは適用できないというエラーが表示されます。
{: tsSymptoms}

フィーチャー・コードの要件を満たしていないアカウントを使用しているか、アカウント内で必要なアクセス権限レベルを持っていません。
{: tsCauses}

- 正しいアカウント・タイプであることを確認してください。例えば、教育割引用のフィーチャー・コードにはライト・アカウントにのみ有効なものがあります。アカウント・タイプを表示するには、**「管理」 > 「アカウント」**と進み、**「アカウント設定」**を選択します。 詳しくは、『[フィーチャー・コードの適用](/docs/account?topic=account-codes)』を参照してください。
- フィーチャー・コードを適用するためのアクセス権限を持っていることを確認してください。フィーチャー・コードを適用するには、すべてのアカウント管理サービスに対するエディター以上の役割を持っている必要があります。役割を検討または変更するには、『[アカウント管理サービスへのアクセス権限の割り当て](/docs/iam?topic=iam-account-services)』を参照してください。
{: tsResolve}
