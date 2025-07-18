---
title: Create and manage access tokens
linkTitle: Access tokens
description: Learn how to create and manage your personal Docker access tokens
  to securely push and pull images programmatically.
keywords: docker hub, hub, security, PAT, personal access token
aliases:
 - /docker-hub/access-tokens/
 - /security/for-developers/access-tokens/
---

You can create a personal access token (PAT) to use as an alternative to your password for Docker CLI authentication.

Compared to passwords, PATs provide the following advantages:

- You can investigate when the PAT was last used and then disable or delete it if you find any suspicious activity.
- When using an access token, you can't perform any administrative activity on the account, including changing the password. It protects your account if your computer is compromised.
- Access tokens are valuable for building integrations, as you can issue multiple tokens, one for each integration, and revoke them at
any time.

## Create an access token

> [!IMPORTANT]
>
> Treat access tokens like your password and keep them secret. Store your tokens securely in a credential manager for example.

Use the Docker Admin Console to create an access token.

1. Sign in to [Docker Home](https://app.docker.com/).
1. Select your avatar in the top-right corner and from the drop-down menu select **Account settings**.
1. Select **Personal access tokens**.
1. Select **Generate new token**.
1. Add a description for your token. Use something that indicates the use case or purpose of the token.
1. Select the expiration date for the token.
1. Set the access permissions.
   The access permissions are scopes that set restrictions in your
   repositories. For example, for Read & Write permissions, an automation
   pipeline can build an image and then push it to a repository. However, it
   can't delete the repository.
1. Select **Generate** and then copy the token that appears on the screen and save it. You won't be able to retrieve the token once you close this prompt.

## Use an access token

You can use an access token in place of your password when you sign in using Docker CLI.

Sign in from your Docker CLI client with the following command, replacing `YOUR_USERNAME` with your Docker ID:

```console
$ docker login --username <YOUR_USERNAME>
```

When prompted for a password, enter your personal access token instead of a password.

> [!NOTE]
>
> If you have [two-factor authentication (2FA)](2fa/_index.md) enabled, you must
> use a personal access token when logging in from the Docker CLI. 2FA is an
> optional, but more secure method of authentication.

### Fair use

When utilizing PATs, users should be aware that excessive creation of PATs could lead to throttling, or additional charges. To ensure fair resource usage and maintain service quality, Docker reserves the right to impose restrictions or apply additional charges to accounts exhibiting excessive use of PATs.

## Modify existing tokens

> [!NOTE]
>
> You can't edit the expiration date on an existing token. You must create a new PAT if you need to set a new expiration date.

You can rename, activate, deactivate, or delete a token as needed. You can manage your tokens in your account settings.

1. Sign in to [Docker Home](https://app.docker.com/login).
1. Select your avatar in the top-right corner and from the drop-down menu select **Account settings**.
1. Select **Personal access tokens**.

   This page shows an overview of all your
   tokens, and lists if the token was generated manually or if it was
   [auto-generated](#auto-generated-tokens). You can also view the scope of the
   tokens, which tokens are activate and inactive, when they were created, when
   they were last used, and their expiration date.
1. Select the actions menu on the far right of a token row, then select **Deactivate** or **Activate**, **Edit**, or **Delete** to modify the token.
1. After editing the token, select **Save token**.

## Auto-generated tokens

When you sign in to your Docker account with Docker Desktop, Docker Desktop generates an authentication token on your behalf. When you interact with Docker Hub using the Docker CLI, the CLI uses this token for authentication. The token scope has Read, Write, and Delete access. If your Docker Desktop session expires, the token is automatically removed locally.

You can have up to 5 auto-generated tokens associated with your account. These are deleted and created automatically based on usage and creation dates. You can also delete your auto-generated tokens as needed. For more information, see [Modify existing tokens](#modify-existing-tokens).
