---
description: SCMProviderGeneratorGitlab defines connection info specific to Gitlab.
layout: schema
name: v1alpha1SCMProviderGeneratorGitlab
properties_list:
- description: Scan all branches instead of just the default branch.
  name: allBranches
  type: boolean
- description: The Gitlab API URL to talk to.
  name: api
  type: string
- description: ''
  name: caRef
  type: object
- description: Gitlab group to scan. Required. You can use either the project id (recommended) or the full namespaced path.
  name: group
  type: string
- description: Include repositories that are archived.
  name: includeArchivedRepos
  type: boolean
- description: ''
  name: includeSharedProjects
  type: boolean
- description: ''
  name: includeSubgroups
  type: boolean
- description: ''
  name: insecure
  type: boolean
- description: ''
  name: tokenRef
  type: object
- description: Filter repos list based on Gitlab Topic.
  name: topic
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-gitlab-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-gitlab
source_filename: argo-cd-v1alpha1-scm-provider-generator-gitlab-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-gitlab-schema.json\",\n  \"title\": \"v1alpha1SCMProviderGeneratorGitlab\",\n  \"description\": \"SCMProviderGeneratorGitlab defines connection info specific to Gitlab.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allBranches\": {\n      \"description\": \"Scan all branches instead of just the default branch.\",\n      \"type\": \"boolean\"\n    },\n    \"api\": {\n      \"description\": \"The Gitlab API URL to talk to.\",\n      \"type\": \"string\"\n    },\n    \"caRef\": {\n      \"$ref\": \"#/definitions/v1alpha1ConfigMapKeyRef\"\n    },\n    \"group\": {\n      \"description\": \"Gitlab group to scan. Required.  You can use either the project id (recommended) or the full namespaced path.\",\n      \"type\": \"string\"\n    },\n    \"includeArchivedRepos\"\
  : {\n      \"description\": \"Include repositories that are archived.\",\n      \"type\": \"boolean\"\n    },\n    \"includeSharedProjects\": {\n      \"type\": \"boolean\",\n      \"title\": \"When recursing through subgroups, also include shared Projects (true) or scan only the subgroups under same path (false).  Defaults to \\\"true\\\"\"\n    },\n    \"includeSubgroups\": {\n      \"type\": \"boolean\",\n      \"title\": \"Recurse through subgroups (true) or scan only the base group (false).  Defaults to \\\"false\\\"\"\n    },\n    \"insecure\": {\n      \"type\": \"boolean\",\n      \"title\": \"Skips validating the SCM provider's TLS certificate - useful for self-signed certificates.; default: false\"\n    },\n    \"tokenRef\": {\n      \"$ref\": \"#/definitions/v1alpha1SecretRef\"\n    },\n    \"topic\": {\n      \"description\": \"Filter repos list based on Gitlab Topic.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-gitlab-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorGitlab
---
