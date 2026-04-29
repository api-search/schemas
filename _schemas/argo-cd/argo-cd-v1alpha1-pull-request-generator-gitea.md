---
description: PullRequestGeneratorGitea defines connection info specific to Gitea.
layout: schema
name: v1alpha1PullRequestGeneratorGitea
properties_list:
- description: ''
  name: api
  type: string
- description: 'Allow insecure tls, for self-signed certificates; default: false.'
  name: insecure
  type: boolean
- description: ''
  name: labels
  type: array
- description: Gitea org or user to scan. Required.
  name: owner
  type: string
- description: Gitea repo name to scan. Required.
  name: repo
  type: string
- description: ''
  name: tokenRef
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-gitea-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-gitea
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-gitea-schema.json\",\n  \"title\": \"v1alpha1PullRequestGeneratorGitea\",\n  \"description\": \"PullRequestGeneratorGitea defines connection info specific to Gitea.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api\": {\n      \"type\": \"string\",\n      \"title\": \"The Gitea API URL to talk to. Required\"\n    },\n    \"insecure\": {\n      \"description\": \"Allow insecure tls, for self-signed certificates; default: false.\",\n      \"type\": \"boolean\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"title\": \"Labels is used to filter the PRs that you want to target\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"owner\": {\n      \"description\": \"Gitea org or user to scan. Required.\",\n      \"type\": \"string\"\
  \n    },\n    \"repo\": {\n      \"description\": \"Gitea repo name to scan. Required.\",\n      \"type\": \"string\"\n    },\n    \"tokenRef\": {\n      \"$ref\": \"#/definitions/v1alpha1SecretRef\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-gitea-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorGitea
---
