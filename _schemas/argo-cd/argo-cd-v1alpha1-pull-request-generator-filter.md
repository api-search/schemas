---
description: PullRequestGeneratorFilter is a single pull request filter. If multiple filter types are set on a single struct, they will be AND'd together. All filters must pass for a pull request to be included.
layout: schema
name: v1alpha1PullRequestGeneratorFilter
properties_list:
- description: ''
  name: branchMatch
  type: string
- description: ''
  name: targetBranchMatch
  type: string
- description: ''
  name: titleMatch
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-filter-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-filter-schema.json\",\n  \"title\": \"v1alpha1PullRequestGeneratorFilter\",\n  \"description\": \"PullRequestGeneratorFilter is a single pull request filter.\\nIf multiple filter types are set on a single struct, they will be AND'd together. All filters must\\npass for a pull request to be included.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branchMatch\": {\n      \"type\": \"string\"\n    },\n    \"targetBranchMatch\": {\n      \"type\": \"string\"\n    },\n    \"titleMatch\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-filter-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorFilter
---
