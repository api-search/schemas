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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-repo-creds-schema.json\",\n  \"title\": \"v1alpha1RepoCreds\",\n  \"description\": \"v1alpha1RepoCreds schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"azureActiveDirectoryEndpoint\": {\n      \"type\": \"string\",\n      \"title\": \"AzureActiveDirectoryEndpoint specifies the Azure Active Directory endpoint used for Service Principal authentication. If empty will default to https://login.microsoftonline.com\"\n    },\n    \"azureServicePrincipalClientId\": {\n      \"type\": \"string\",\n      \"title\": \"AzureServicePrincipalClientId specifies the client ID of the Azure Service Principal used to access the repo\"\n    },\n    \"azureServicePrincipalClientSecret\": {\n      \"type\": \"string\",\n      \"title\": \"AzureServicePrincipalClientSecret specifies the\
  \ client secret of the Azure Service Principal used to access the repo\"\n    },\n    \"azureServicePrincipalTenantId\": {\n      \"type\": \"string\",\n      \"title\": \"AzureServicePrincipalTenantId specifies the tenant ID of the Azure Service Principal used to access the repo\"\n    },\n    \"bearerToken\": {\n      \"type\": \"string\",\n      \"title\": \"BearerToken contains the bearer token used for Git BitBucket Data Center auth at the repo server\"\n    },\n    \"enableOCI\": {\n      \"type\": \"boolean\",\n      \"title\": \"EnableOCI specifies whether helm-oci support should be enabled for this repo\"\n    },\n    \"forceHttpBasicAuth\": {\n      \"type\": \"boolean\",\n      \"title\": \"ForceHttpBasicAuth specifies whether Argo CD should attempt to force basic auth for HTTP connections\"\n    },\n    \"gcpServiceAccountKey\": {\n      \"type\": \"string\",\n      \"title\": \"GCPServiceAccountKey specifies the service account key in JSON format to be used for getting credentials\
  \ to Google Cloud Source repos\"\n    },\n    \"githubAppEnterpriseBaseUrl\": {\n      \"type\": \"string\",\n      \"title\": \"GithubAppEnterpriseBaseURL specifies the GitHub API URL for GitHub app authentication. If empty will default to https://api.github.com\"\n    },\n    \"githubAppID\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"GithubAppId specifies the Github App ID of the app used to access the repo for GitHub app authentication\"\n    },\n    \"githubAppInstallationID\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"GithubAppInstallationId specifies the ID of the installed GitHub App for GitHub app authentication\"\n    },\n    \"githubAppPrivateKey\": {\n      \"type\": \"string\",\n      \"title\": \"GithubAppPrivateKey specifies the private key PEM data for authentication via GitHub app\"\n    },\n    \"insecureOCIForceHttp\": {\n      \"description\": \"InsecureOCIForceHttp specifies whether the\
  \ connection to the repository uses TLS at _all_. If true, no TLS. This flag is applicable for OCI repos only.\",\n      \"type\": \"boolean\"\n    },\n    \"noProxy\": {\n      \"type\": \"string\",\n      \"title\": \"NoProxy specifies a list of targets where the proxy isn't used, applies only in cases where the proxy is applied\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"title\": \"Password for authenticating at the repo server\"\n    },\n    \"proxy\": {\n      \"type\": \"string\",\n      \"title\": \"Proxy specifies the HTTP/HTTPS proxy used to access repos at the repo server\"\n    },\n    \"sshPrivateKey\": {\n      \"type\": \"string\",\n      \"title\": \"SSHPrivateKey contains the private key data for authenticating at the repo server using SSH (only Git repos)\"\n    },\n    \"tlsClientCertData\": {\n      \"type\": \"string\",\n      \"title\": \"TLSClientCertData specifies the TLS client cert data for authenticating at the repo server\"\n    },\n\
  \    \"tlsClientCertKey\": {\n      \"type\": \"string\",\n      \"title\": \"TLSClientCertKey specifies the TLS client cert key for authenticating at the repo server\"\n    },\n    \"type\": {\n      \"description\": \"Type specifies the type of the repoCreds. Can be either \\\"git\\\", \\\"helm\\\" or \\\"oci\\\". \\\"git\\\" is assumed if empty or absent.\",\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"title\": \"URL is the URL to which these credentials match\"\n    },\n    \"useAzureWorkloadIdentity\": {\n      \"type\": \"boolean\",\n      \"title\": \"UseAzureWorkloadIdentity specifies whether to use Azure Workload Identity for authentication\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"title\": \"Username for authenticating at the repo server\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-repo-creds-schema.json
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
