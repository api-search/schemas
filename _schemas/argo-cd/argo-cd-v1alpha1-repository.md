---
description: v1alpha1Repository schema from Argo CD API
layout: schema
name: v1alpha1Repository
properties_list:
- description: ''
  name: azureActiveDirectoryEndpoint
  type: string
- description: ''
  name: azureServicePrincipalClientId
  type: string
- description: ''
  name: azureServicePrincipalClientSecret
  type: string
- description: ''
  name: azureServicePrincipalTenantId
  type: string
- description: ''
  name: bearerToken
  type: string
- description: ''
  name: connectionState
  type: object
- description: Depth specifies the depth for shallow clones. A value of 0 or omitting the field indicates a full clone.
  name: depth
  type: integer
- description: EnableLFS specifies whether git-lfs support should be enabled for this repo. Only valid for Git repositories.
  name: enableLfs
  type: boolean
- description: ''
  name: enableOCI
  type: boolean
- description: ''
  name: forceHttpBasicAuth
  type: boolean
- description: ''
  name: gcpServiceAccountKey
  type: string
- description: ''
  name: githubAppEnterpriseBaseUrl
  type: string
- description: ''
  name: githubAppID
  type: integer
- description: ''
  name: githubAppInstallationID
  type: integer
- description: ''
  name: githubAppPrivateKey
  type: string
- description: ''
  name: inheritedCreds
  type: boolean
- description: ''
  name: insecure
  type: boolean
- description: ''
  name: insecureIgnoreHostKey
  type: boolean
- description: InsecureOCIForceHttp specifies whether the connection to the repository uses TLS at _all_. If true, no TLS. This flag is applicable for OCI repos only.
  name: insecureOCIForceHttp
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: noProxy
  type: string
- description: ''
  name: password
  type: string
- description: ''
  name: project
  type: string
- description: ''
  name: proxy
  type: string
- description: ''
  name: repo
  type: string
- description: SSHPrivateKey contains the PEM data for authenticating at the repo server. Only used with Git repos.
  name: sshPrivateKey
  type: string
- description: ''
  name: tlsClientCertData
  type: string
- description: ''
  name: tlsClientCertKey
  type: string
- description: Type specifies the type of the repo. Can be either "git" or "helm. "git" is assumed if empty or absent.
  name: type
  type: string
- description: ''
  name: useAzureWorkloadIdentity
  type: boolean
- description: ''
  name: username
  type: string
- description: WebhookManifestCacheWarmDisabled disables manifest cache warming during webhook processing for this repository. When set, webhook handlers will only trigger reconciliation for affected applications an
  name: webhookManifestCacheWarmDisabled
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-repository-schema.json
slug: argo-cd-v1alpha1-repository
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1Repository
---
