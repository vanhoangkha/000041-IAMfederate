---
title : "Create Identity providers on AWS"
date : "`r Sys.Date()`"
weight : 5
chapter : false
pre : " <b> 5. </b> "
---

1. Sign in to [AWS Console](https://aws.amazon.com/en/console/)

![Identity providers](/images/5-Identityproviders/0001-identityprovider.png)

2. Find **IAM** and select the **Identity and Access Management (IAM)** interface
3. Select **Identity providers**

![Identity providers](/images/5-Identityproviders/0002-identityprovider.png)

4. Create Identity Provider, select **Add provider**

![Identity providers](/images/5-Identityproviders/0003-identityprovider.png)

5. In **Add an Identity provider**, section **Configure provider**

- **Provider type**, select **SAML**
- **Provider name**, enter ```AzureAD```
- **Metadata document**, select **Choose file** and upload metadata file **AWS Single-Account Access.xml**

![Identity providers](/images/5-Identityproviders/0004-identityprovider.png)

6. Select **Add provider**

![Identity providers](/images/5-Identityproviders/0005-identityprovider.png)

7. Select **View provider** to view details.

![Identity providers](/images/5-Identityproviders/0006-identityprovider.png)

8. We have successfully created AzureAD Identity Provider on AWS.

![Identity providers](/images/5-Identityproviders/0007-identityprovider.png)