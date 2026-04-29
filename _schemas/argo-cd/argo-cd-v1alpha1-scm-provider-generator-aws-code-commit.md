---
description: SCMProviderGeneratorAWSCodeCommit defines connection info specific to AWS CodeCommit.
layout: schema
name: v1alpha1SCMProviderGeneratorAWSCodeCommit
properties_list:
- description: Scan all branches instead of just the default branch.
  name: allBranches
  type: boolean
- description: Region provides the AWS region to discover repos. if not provided, AppSet controller will infer the current region from environment.
  name: region
  type: string
- description: Role provides the AWS IAM role to assume, for cross-account repo discovery if not provided, AppSet controller will use its pod/node identity to discover.
  name: role
  type: string
- description: ''
  name: tagFilters
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-aws-code-commit-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-aws-code-commit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-aws-code-commit-schema.json\",\n  \"title\": \"v1alpha1SCMProviderGeneratorAWSCodeCommit\",\n  \"description\": \"SCMProviderGeneratorAWSCodeCommit defines connection info specific to AWS CodeCommit.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allBranches\": {\n      \"description\": \"Scan all branches instead of just the default branch.\",\n      \"type\": \"boolean\"\n    },\n    \"region\": {\n      \"description\": \"Region provides the AWS region to discover repos.\\nif not provided, AppSet controller will infer the current region from environment.\",\n      \"type\": \"string\"\n    },\n    \"role\": {\n      \"description\": \"Role provides the AWS IAM role to assume, for cross-account repo discovery\\nif not provided, AppSet controller will use its pod/node\
  \ identity to discover.\",\n      \"type\": \"string\"\n    },\n    \"tagFilters\": {\n      \"type\": \"array\",\n      \"title\": \"TagFilters provides the tag filter(s) for repo discovery\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1TagFilter\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-aws-code-commit-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorAWSCodeCommit
---
