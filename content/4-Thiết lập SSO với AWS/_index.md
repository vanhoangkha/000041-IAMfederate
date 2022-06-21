---
title : "Setting up SSO with AWS"
date : "`r Sys.Date()`"
weight : 4
chapter : false
pre : " <b> 4. </b> "
---

1. In the **AWS Single-Account Access** page, on the left menu, select **Single sign on**

![Set Up SSO with AWS](/images/4-SSO/0001-sso.png)

2. Select **SAML**

![Set Up SSO with AWS](/images/4-SSO/0002-sso.png)

3. In the **Set up Single Sign-On with SAML** section

- Section **Basic SAML Configuration**, select **Edit**


![Set Up SSO with AWS](/images/4-SSO/0003-sso.png)


4. Section **Basic SAML Configuration**

- **Identifier (Entity ID)**, add **#2** to the link to make sure this **SAML** login link is unique. Because I already have a **SAML** in my account, I have to edit the link here.


![Set Up SSO with AWS](/images/4-SSO/0004-sso.png)

5. Select **Save** to save the information

![Set Up SSO with AWS](/images/4-SSO/0005-sso.png)

6. You download **Federation Metadata XML**, you will use this XML file to upload to AWS to connect.

![Set Up SSO with AWS](/images/4-SSO/0006-sso.png)