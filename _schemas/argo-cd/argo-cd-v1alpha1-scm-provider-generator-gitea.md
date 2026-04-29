---
description: SCMProviderGeneratorGitea defines a connection info specific to Gitea.
layout: schema
name: v1alpha1SCMProviderGeneratorGitea
properties_list:
- description: Scan all branches instead of just the default branch.
  name: allBranches
  type: boolean
- description: The Gitea URL to talk to. For example https://gitea.mydomain.com/.
  name: api
  type: string
- description: Exclude repositories that are archived.
  name: excludeArchivedRepos
  type: boolean
- description: ''
  name: insecure
  type: boolean
- description: Gitea organization or user to scan. Required.
  name: owner
  type: string
- description: ''
  name: tokenRef
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-gitea-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-gitea
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-gitea-schema.json\",\n  \"title\": \"v1alpha1SCMProviderGeneratorGitea\",\n  \"description\": \"SCMProviderGeneratorGitea defines a connection info specific to Gitea.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allBranches\": {\n      \"description\": \"Scan all branches instead of just the default branch.\",\n      \"type\": \"boolean\"\n    },\n    \"api\": {\n      \"description\": \"The Gitea URL to talk to. For example https://gitea.mydomain.com/.\",\n      \"type\": \"string\"\n    },\n    \"excludeArchivedRepos\": {\n      \"description\": \"Exclude repositories that are archived.\",\n      \"type\": \"boolean\"\n    },\n    \"insecure\": {\n      \"type\": \"boolean\",\n      \"title\": \"Allow self-signed TLS / Certificates; default: false\"\n    },\n\
  \    \"owner\": {\n      \"description\": \"Gitea organization or user to scan. Required.\",\n      \"type\": \"string\"\n    },\n    \"tokenRef\": {\n      \"$ref\": \"#/definitions/v1alpha1SecretRef\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-gitea-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorGitea
---
