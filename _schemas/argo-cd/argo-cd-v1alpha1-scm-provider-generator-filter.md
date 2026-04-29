---
description: SCMProviderGeneratorFilter is a single repository filter. If multiple filter types are set on a single struct, they will be AND'd together. All filters must pass for a repo to be included.
layout: schema
name: v1alpha1SCMProviderGeneratorFilter
properties_list:
- description: A regex which must match the branch name.
  name: branchMatch
  type: string
- description: A regex which must match at least one label.
  name: labelMatch
  type: string
- description: An array of paths, all of which must not exist.
  name: pathsDoNotExist
  type: array
- description: An array of paths, all of which must exist.
  name: pathsExist
  type: array
- description: A regex for repo names.
  name: repositoryMatch
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-filter-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-filter
source_filename: argo-cd-v1alpha1-scm-provider-generator-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-filter-schema.json\",\n  \"title\": \"v1alpha1SCMProviderGeneratorFilter\",\n  \"description\": \"SCMProviderGeneratorFilter is a single repository filter.\\nIf multiple filter types are set on a single struct, they will be AND'd together. All filters must\\npass for a repo to be included.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branchMatch\": {\n      \"description\": \"A regex which must match the branch name.\",\n      \"type\": \"string\"\n    },\n    \"labelMatch\": {\n      \"description\": \"A regex which must match at least one label.\",\n      \"type\": \"string\"\n    },\n    \"pathsDoNotExist\": {\n      \"description\": \"An array of paths, all of which must not exist.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\
  \n      }\n    },\n    \"pathsExist\": {\n      \"description\": \"An array of paths, all of which must exist.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"repositoryMatch\": {\n      \"description\": \"A regex for repo names.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-filter-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorFilter
---
