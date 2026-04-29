---
description: PullRequestGeneratorGitLab defines connection info specific to GitLab.
layout: schema
name: v1alpha1PullRequestGeneratorGitLab
properties_list:
- description: The GitLab API URL to talk to. If blank, uses https://gitlab.com/.
  name: api
  type: string
- description: ''
  name: caRef
  type: object
- description: ''
  name: insecure
  type: boolean
- description: ''
  name: labels
  type: array
- description: GitLab project to scan. Required.
  name: project
  type: string
- description: 'PullRequestState is an additional MRs filter to get only those with a certain state. Default: "" (all states). Valid values: opened, closed, merged, locked".'
  name: pullRequestState
  type: string
- description: ''
  name: tokenRef
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-git-lab-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-git-lab
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-git-lab-schema.json\",\n  \"title\": \"v1alpha1PullRequestGeneratorGitLab\",\n  \"description\": \"PullRequestGeneratorGitLab defines connection info specific to GitLab.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api\": {\n      \"description\": \"The GitLab API URL to talk to. If blank, uses https://gitlab.com/.\",\n      \"type\": \"string\"\n    },\n    \"caRef\": {\n      \"$ref\": \"#/definitions/v1alpha1ConfigMapKeyRef\"\n    },\n    \"insecure\": {\n      \"type\": \"boolean\",\n      \"title\": \"Skips validating the SCM provider's TLS certificate - useful for self-signed certificates.; default: false\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"title\": \"Labels is used to filter the MRs that you want to target\",\n      \"items\"\
  : {\n        \"type\": \"string\"\n      }\n    },\n    \"project\": {\n      \"description\": \"GitLab project to scan. Required.\",\n      \"type\": \"string\"\n    },\n    \"pullRequestState\": {\n      \"description\": \"PullRequestState is an additional MRs filter to get only those with a certain state. Default: \\\"\\\" (all states).\\nValid values: opened, closed, merged, locked\\\".\",\n      \"type\": \"string\"\n    },\n    \"tokenRef\": {\n      \"$ref\": \"#/definitions/v1alpha1SecretRef\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-git-lab-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorGitLab
---
