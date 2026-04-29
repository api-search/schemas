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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-repository-schema.json\",\n  \"title\": \"v1alpha1Repository\",\n  \"description\": \"v1alpha1Repository schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"azureActiveDirectoryEndpoint\": {\n      \"type\": \"string\",\n      \"title\": \"AzureActiveDirectoryEndpoint specifies the Azure Active Directory endpoint used for Service Principal authentication. If empty will default to https://login.microsoftonline.com\"\n    },\n    \"azureServicePrincipalClientId\": {\n      \"type\": \"string\",\n      \"title\": \"AzureServicePrincipalClientId specifies the client ID of the Azure Service Principal used to access the repo\"\n    },\n    \"azureServicePrincipalClientSecret\": {\n      \"type\": \"string\",\n      \"title\": \"AzureServicePrincipalClientSecret specifies\
  \ the client secret of the Azure Service Principal used to access the repo\"\n    },\n    \"azureServicePrincipalTenantId\": {\n      \"type\": \"string\",\n      \"title\": \"AzureServicePrincipalTenantId specifies the tenant ID of the Azure Service Principal used to access the repo\"\n    },\n    \"bearerToken\": {\n      \"type\": \"string\",\n      \"title\": \"BearerToken contains the bearer token used for Git BitBucket Data Center auth at the repo server\"\n    },\n    \"connectionState\": {\n      \"$ref\": \"#/definitions/v1alpha1ConnectionState\"\n    },\n    \"depth\": {\n      \"description\": \"Depth specifies the depth for shallow clones. A value of 0 or omitting the field indicates a full clone.\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"enableLfs\": {\n      \"description\": \"EnableLFS specifies whether git-lfs support should be enabled for this repo. Only valid for Git repositories.\",\n      \"type\": \"boolean\"\n    },\n    \"enableOCI\"\
  : {\n      \"type\": \"boolean\",\n      \"title\": \"EnableOCI specifies whether helm-oci support should be enabled for this repo\"\n    },\n    \"forceHttpBasicAuth\": {\n      \"type\": \"boolean\",\n      \"title\": \"ForceHttpBasicAuth specifies whether Argo CD should attempt to force basic auth for HTTP connections\"\n    },\n    \"gcpServiceAccountKey\": {\n      \"type\": \"string\",\n      \"title\": \"GCPServiceAccountKey specifies the service account key in JSON format to be used for getting credentials to Google Cloud Source repos\"\n    },\n    \"githubAppEnterpriseBaseUrl\": {\n      \"type\": \"string\",\n      \"title\": \"GithubAppEnterpriseBaseURL specifies the base URL of GitHub Enterprise installation. If empty will default to https://api.github.com\"\n    },\n    \"githubAppID\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"GithubAppId specifies the ID of the GitHub app used to access the repo\"\n    },\n    \"githubAppInstallationID\"\
  : {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"GithubAppInstallationId specifies the installation ID of the GitHub App used to access the repo\"\n    },\n    \"githubAppPrivateKey\": {\n      \"type\": \"string\",\n      \"title\": \"Github App Private Key PEM data\"\n    },\n    \"inheritedCreds\": {\n      \"type\": \"boolean\",\n      \"title\": \"Whether credentials were inherited from a credential set\"\n    },\n    \"insecure\": {\n      \"type\": \"boolean\",\n      \"title\": \"Insecure specifies whether the connection to the repository ignores any errors when verifying TLS certificates or SSH host keys\"\n    },\n    \"insecureIgnoreHostKey\": {\n      \"type\": \"boolean\",\n      \"title\": \"InsecureIgnoreHostKey should not be used anymore, Insecure is favoured\\nUsed only for Git repos\"\n    },\n    \"insecureOCIForceHttp\": {\n      \"description\": \"InsecureOCIForceHttp specifies whether the connection to the repository uses TLS at\
  \ _all_. If true, no TLS. This flag is applicable for OCI repos only.\",\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name specifies a name to be used for this repo. Only used with Helm repos\"\n    },\n    \"noProxy\": {\n      \"type\": \"string\",\n      \"title\": \"NoProxy specifies a list of targets where the proxy isn't used, applies only in cases where the proxy is applied\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"title\": \"Password contains the password or PAT used for authenticating at the remote repository\"\n    },\n    \"project\": {\n      \"type\": \"string\",\n      \"title\": \"Reference between project and repository that allows it to be automatically added as an item inside SourceRepos project entity\"\n    },\n    \"proxy\": {\n      \"type\": \"string\",\n      \"title\": \"Proxy specifies the HTTP/HTTPS proxy used to access the repo\"\n    },\n    \"repo\": {\n      \"type\": \"\
  string\",\n      \"title\": \"Repo contains the URL to the remote repository\"\n    },\n    \"sshPrivateKey\": {\n      \"description\": \"SSHPrivateKey contains the PEM data for authenticating at the repo server. Only used with Git repos.\",\n      \"type\": \"string\"\n    },\n    \"tlsClientCertData\": {\n      \"type\": \"string\",\n      \"title\": \"TLSClientCertData contains a certificate in PEM format for authenticating at the repo server\"\n    },\n    \"tlsClientCertKey\": {\n      \"type\": \"string\",\n      \"title\": \"TLSClientCertKey contains a private key in PEM format for authenticating at the repo server\"\n    },\n    \"type\": {\n      \"description\": \"Type specifies the type of the repo. Can be either \\\"git\\\" or \\\"helm. \\\"git\\\" is assumed if empty or absent.\",\n      \"type\": \"string\"\n    },\n    \"useAzureWorkloadIdentity\": {\n      \"type\": \"boolean\",\n      \"title\": \"UseAzureWorkloadIdentity specifies whether to use Azure Workload Identity\
  \ for authentication\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"title\": \"Username contains the user name used for authenticating at the remote repository\"\n    },\n    \"webhookManifestCacheWarmDisabled\": {\n      \"description\": \"WebhookManifestCacheWarmDisabled disables manifest cache warming during webhook processing for this repository.\\nWhen set, webhook handlers will only trigger reconciliation for affected applications and skip Redis cache\\noperations for unaffected ones. Recommended for large monorepos with plain YAML manifests.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-repository-schema.json
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
