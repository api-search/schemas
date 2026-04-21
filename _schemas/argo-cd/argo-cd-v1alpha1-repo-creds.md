---
description: v1alpha1RepoCreds schema from Argo CD API
layout: schema
name: v1alpha1RepoCreds
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
- description: InsecureOCIForceHttp specifies whether the connection to the repository uses TLS at _all_. If true, no TLS. This flag is applicable for OCI repos only.
  name: insecureOCIForceHttp
  type: boolean
- description: ''
  name: noProxy
  type: string
- description: ''
  name: password
  type: string
- description: ''
  name: proxy
  type: string
- description: ''
  name: sshPrivateKey
  type: string
- description: ''
  name: tlsClientCertData
  type: string
- description: ''
  name: tlsClientCertKey
  type: string
- description: Type specifies the type of the repoCreds. Can be either "git", "helm" or "oci". "git" is assumed if empty or absent.
  name: type
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: useAzureWorkloadIdentity
  type: boolean
- description: ''
  name: username
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-repo-creds-schema.json
slug: argo-cd-v1alpha1-repo-creds
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1RepoCreds
---
