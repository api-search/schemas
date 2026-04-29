---
description: PullRequestGeneratorGithub defines connection info specific to GitHub.
layout: schema
name: v1alpha1PullRequestGeneratorGithub
properties_list:
- description: The GitHub API URL to talk to. If blank, use https://api.github.com/.
  name: api
  type: string
- description: AppSecretName is a reference to a GitHub App repo-creds secret with permission to access pull requests.
  name: appSecretName
  type: string
- description: ''
  name: labels
  type: array
- description: GitHub org or user to scan. Required.
  name: owner
  type: string
- description: GitHub repo name to scan. Required.
  name: repo
  type: string
- description: ''
  name: tokenRef
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-github-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-github
source_filename: argo-cd-v1alpha1-pull-request-generator-github-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-github-schema.json\",\n  \"title\": \"v1alpha1PullRequestGeneratorGithub\",\n  \"description\": \"PullRequestGeneratorGithub defines connection info specific to GitHub.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api\": {\n      \"description\": \"The GitHub API URL to talk to. If blank, use https://api.github.com/.\",\n      \"type\": \"string\"\n    },\n    \"appSecretName\": {\n      \"description\": \"AppSecretName is a reference to a GitHub App repo-creds secret with permission to access pull requests.\",\n      \"type\": \"string\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"title\": \"Labels is used to filter the PRs that you want to target\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"owner\": {\n   \
  \   \"description\": \"GitHub org or user to scan. Required.\",\n      \"type\": \"string\"\n    },\n    \"repo\": {\n      \"description\": \"GitHub repo name to scan. Required.\",\n      \"type\": \"string\"\n    },\n    \"tokenRef\": {\n      \"$ref\": \"#/definitions/v1alpha1SecretRef\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-github-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorGithub
---
