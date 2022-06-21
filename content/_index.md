---
title : "AWS IAM Federation from Microsoft Azure Active Directory"
date : "`r Sys.Date()`"
weight : 1
chapter : false
---
# AWS IAM Federation from Microsoft Azure Active Directory

### Overview

In this lab, we will learn about the IAM Federation feature on AWS. An abstract concept for those who are just starting to learn about AWS.

Results of this lab:

1. Integrating Microsoft Azure AD with IAM via SAML

2. Users created on Microsoft Azure AD have the ability to connect to AWS to use the permissions set up on both AWS and Azure sides.

3. Understanding IAM Federation

### Concept of SAML

- SAML stands for **Security Assertion Markup language**.
- Generally, users need to enter username and password to log in to any application.
- SAML is a technique to achieve **Single Sign-On** – Single Sign On (SSO).
- **Security Assertion Markup Language** (SAML) is an Xml-based framework that allows identity providers to provide authorization credentials to service providers.
- With SAML, you need to enter a security attribute to log in to the application
- SAML is the link between user identity authentication and service authorization.
- SAML provides a service called Single Sign On which means the user has to sign in once and can use the same credentials to sign in to another service provider.
  
### Content

1. [Introduction]()
2. [Preparation steps]()
3. [Initiate Azure AD]()
4. [Create Azure AD Users]()
5. [Create an Enterprise Application (EA) connecting to AWS]()
6. [Set Up SSO with AWS]()
7. [Create Identity Provider on AWS]()
8. [Sync Roles on AWS to Azure AD assume]()
9. [Federating Azure AD Users Accessing AWS]()
10. [Federating Azure AD Users to AWS]()
11. [Check Service Usage]()