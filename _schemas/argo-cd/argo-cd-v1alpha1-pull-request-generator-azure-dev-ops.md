---
description: PullRequestGeneratorAzureDevOps defines connection info specific to AzureDevOps.
layout: schema
name: v1alpha1PullRequestGeneratorAzureDevOps
properties_list:
- description: The Azure DevOps API URL to talk to. If blank, use https://dev.azure.com/.
  name: api
  type: string
- description: ''
  name: labels
  type: array
- description: Azure DevOps org to scan. Required.
  name: organization
  type: string
- description: Azure DevOps project name to scan. Required.
  name: project
  type: string
- description: Azure DevOps repo name to scan. Required.
  name: repo
  type: string
- description: ''
  name: tokenRef
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-azure-dev-ops-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-azure-dev-ops
source_filename: argo-cd-v1alpha1-pull-request-generator-azure-dev-ops-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-azure-dev-ops-schema.json\",\n  \"title\": \"v1alpha1PullRequestGeneratorAzureDevOps\",\n  \"description\": \"PullRequestGeneratorAzureDevOps defines connection info specific to AzureDevOps.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api\": {\n      \"description\": \"The Azure DevOps API URL to talk to. If blank, use https://dev.azure.com/.\",\n      \"type\": \"string\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"title\": \"Labels is used to filter the PRs that you want to target\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"organization\": {\n      \"description\": \"Azure DevOps org to scan. Required.\",\n      \"type\": \"string\"\n    },\n    \"project\": {\n      \"description\": \"Azure DevOps project\
  \ name to scan. Required.\",\n      \"type\": \"string\"\n    },\n    \"repo\": {\n      \"description\": \"Azure DevOps repo name to scan. Required.\",\n      \"type\": \"string\"\n    },\n    \"tokenRef\": {\n      \"$ref\": \"#/definitions/v1alpha1SecretRef\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-azure-dev-ops-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorAzureDevOps
---
