---
description: SCMProviderGeneratorGithub defines connection info specific to GitHub.
layout: schema
name: v1alpha1SCMProviderGeneratorGithub
properties_list:
- description: Scan all branches instead of just the default branch.
  name: allBranches
  type: boolean
- description: The GitHub API URL to talk to. If blank, use https://api.github.com/.
  name: api
  type: string
- description: AppSecretName is a reference to a GitHub App repo-creds secret.
  name: appSecretName
  type: string
- description: Exclude repositories that are archived.
  name: excludeArchivedRepos
  type: boolean
- description: GitHub org to scan. Required.
  name: organization
  type: string
- description: ''
  name: tokenRef
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-github-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-github
source_filename: argo-cd-v1alpha1-scm-provider-generator-github-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-github-schema.json\",\n  \"title\": \"v1alpha1SCMProviderGeneratorGithub\",\n  \"description\": \"SCMProviderGeneratorGithub defines connection info specific to GitHub.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allBranches\": {\n      \"description\": \"Scan all branches instead of just the default branch.\",\n      \"type\": \"boolean\"\n    },\n    \"api\": {\n      \"description\": \"The GitHub API URL to talk to. If blank, use https://api.github.com/.\",\n      \"type\": \"string\"\n    },\n    \"appSecretName\": {\n      \"description\": \"AppSecretName is a reference to a GitHub App repo-creds secret.\",\n      \"type\": \"string\"\n    },\n    \"excludeArchivedRepos\": {\n      \"description\": \"Exclude repositories that are archived.\",\n      \"type\"\
  : \"boolean\"\n    },\n    \"organization\": {\n      \"description\": \"GitHub org to scan. Required.\",\n      \"type\": \"string\"\n    },\n    \"tokenRef\": {\n      \"$ref\": \"#/definitions/v1alpha1SecretRef\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-github-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorGithub
---
