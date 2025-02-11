# GitHub Auth

First, you'll need to create a GitHub OAuth app for your organisation.

## Creating a GitHub OAuth app

From GitHub, click on your profile picture and chose "Settings":

![Step 1](/nx-cloud/enterprise/on-premise/images/github_auth_step_1.png)

Then "Developer settings" from the left-hand menu:

![Step 2](/nx-cloud/enterprise/on-premise/images/github_auth_step_2.png)

Then "OAuth Apps":

![Step 3](/nx-cloud/enterprise/on-premise/images/github_auth_step_3.png)

And create a new OAuth app:

![Step 4](/nx-cloud/enterprise/on-premise/images/github_auth_step_4.png)

Give it a name, and a homepage URL. The authorization callback is the important bit. It needs to be in this form:

```
[your-nx-cloud-url]/auth-callback

# for example
https://my.nx-enterprise.url:8080/auth-callback
```

![Step 5](/nx-cloud/enterprise/on-premise/images/github_auth_step_5.png)

Once you create, keep a note of the Client ID:

![Step 6](/nx-cloud/enterprise/on-premise/images/github_auth_step_6.png)

And then generate a new client secret, and save it somewhere secure (we'll use it in a bit):

![Step 7](/nx-cloud/enterprise/on-premise/images/github_auth_step_7.png)

## Configure Nx Cloud Installation

It's now time to enable auth on NxCloud. Refer to the [auth guide](https://github.com/nrwl/nx-cloud-helm/blob/main/AUTH-GUIDE.md) here for instructions on configuring your Helm values file.

## On Premise Docs

- [Set up Nx Cloud On-Premise](/ci/recipes/enterprise/on-premise/on-premise)
- [Authenticate with a Single Admin](/ci/recipes/enterprise/on-premise/auth-single-admin)
- [Authenticate with GitHub](/ci/recipes/enterprise/on-premise/auth-github)
- [On-Prem VM Setup](/ci/recipes/enterprise/on-premise/ami-setup)
- [Authenticate with GitLab](/ci/recipes/enterprise/on-premise/auth-gitlab)
- [Authenticate with BitBucket](/ci/recipes/enterprise/on-premise/auth-bitbucket)
- [Authenticate with BitBucket Data Center](/ci/recipes/enterprise/on-premise/auth-bitbucket-data-center)
- [Authenticate via SAML](/ci/recipes/enterprise/on-premise/auth-saml)
- [Advanced Configuration](/ci/recipes/enterprise/on-premise/advanced-config)
- [Custom GitHub App](/ci/recipes/enterprise/on-premise/custom-github-app)
