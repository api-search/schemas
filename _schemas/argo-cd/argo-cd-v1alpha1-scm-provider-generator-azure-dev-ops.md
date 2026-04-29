---
description: SCMProviderGeneratorAzureDevOps defines connection info specific to Azure DevOps.
layout: schema
name: v1alpha1SCMProviderGeneratorAzureDevOps
properties_list:
- description: ''
  name: accessTokenRef
  type: object
- description: Scan all branches instead of just the default branch.
  name: allBranches
  type: boolean
- description: The URL to Azure DevOps. If blank, use https://dev.azure.com.
  name: api
  type: string
- description: Azure Devops organization. Required. E.g. "my-organization".
  name: organization
  type: string
- description: Azure Devops team project. Required. E.g. "my-team".
  name: teamProject
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-azure-dev-ops-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-azure-dev-ops
source_filename: argo-cd-v1alpha1-scm-provider-generator-azure-dev-ops-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-azure-dev-ops-schema.json\",\n  \"title\": \"v1alpha1SCMProviderGeneratorAzureDevOps\",\n  \"description\": \"SCMProviderGeneratorAzureDevOps defines connection info specific to Azure DevOps.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessTokenRef\": {\n      \"$ref\": \"#/definitions/v1alpha1SecretRef\"\n    },\n    \"allBranches\": {\n      \"description\": \"Scan all branches instead of just the default branch.\",\n      \"type\": \"boolean\"\n    },\n    \"api\": {\n      \"description\": \"The URL to Azure DevOps. If blank, use https://dev.azure.com.\",\n      \"type\": \"string\"\n    },\n    \"organization\": {\n      \"description\": \"Azure Devops organization. Required. E.g. \\\"my-organization\\\".\",\n      \"type\": \"string\"\n    },\n    \"\
  teamProject\": {\n      \"description\": \"Azure Devops team project. Required. E.g. \\\"my-team\\\".\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-azure-dev-ops-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorAzureDevOps
---
