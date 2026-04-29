---
description: SCMProviderGeneratorBitbucket defines connection info specific to Bitbucket Cloud (API version 2).
layout: schema
name: v1alpha1SCMProviderGeneratorBitbucket
properties_list:
- description: Scan all branches instead of just the main branch.
  name: allBranches
  type: boolean
- description: ''
  name: appPasswordRef
  type: object
- description: Bitbucket workspace to scan. Required.
  name: owner
  type: string
- description: ''
  name: user
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-bitbucket-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-bitbucket
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-bitbucket-schema.json\",\n  \"title\": \"v1alpha1SCMProviderGeneratorBitbucket\",\n  \"description\": \"SCMProviderGeneratorBitbucket defines connection info specific to Bitbucket Cloud (API version 2).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allBranches\": {\n      \"description\": \"Scan all branches instead of just the main branch.\",\n      \"type\": \"boolean\"\n    },\n    \"appPasswordRef\": {\n      \"$ref\": \"#/definitions/v1alpha1SecretRef\"\n    },\n    \"owner\": {\n      \"description\": \"Bitbucket workspace to scan. Required.\",\n      \"type\": \"string\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"title\": \"Bitbucket user to use when authenticating.  Should have a \\\"member\\\" role to be able to read all repositories\
  \ and branches.  Required\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-bitbucket-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorBitbucket
---
