---
description: Git or Helm chart source for the application manifests.
layout: schema
name: ApplicationSource
properties_list:
- description: URL of the Git repository or Helm chart repository.
  name: repoURL
  type: string
- description: Path within the repository where manifests are located. Used for Git repositories.
  name: path
  type: string
- description: Git branch, tag, or commit SHA to deploy. Defaults to HEAD.
  name: targetRevision
  type: string
- description: Helm chart name. Used when repoURL points to a Helm registry.
  name: chart
  type: string
- description: Helm-specific source configuration.
  name: helm
  type: object
- description: Kustomize-specific source configuration.
  name: kustomize
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-application-source-schema.json
slug: argo-cd-application-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-application-source-schema.json\",\n  \"title\": \"ApplicationSource\",\n  \"description\": \"Git or Helm chart source for the application manifests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repoURL\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the Git repository or Helm chart repository.\",\n      \"format\": \"uri\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Path within the repository where manifests are located. Used for Git repositories.\"\n    },\n    \"targetRevision\": {\n      \"type\": \"string\",\n      \"description\": \"Git branch, tag, or commit SHA to deploy. Defaults to HEAD.\"\n    },\n    \"chart\": {\n      \"type\": \"string\",\n      \"description\": \"Helm chart name. Used when repoURL points to a Helm registry.\"\
  \n    },\n    \"helm\": {\n      \"type\": \"object\",\n      \"description\": \"Helm-specific source configuration.\",\n      \"properties\": {\n        \"valueFiles\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"List of Helm value file paths.\"\n        },\n        \"values\": {\n          \"type\": \"string\",\n          \"description\": \"Inline Helm values as a YAML string.\"\n        },\n        \"releaseName\": {\n          \"type\": \"string\",\n          \"description\": \"Helm release name override.\"\n        }\n      }\n    },\n    \"kustomize\": {\n      \"type\": \"object\",\n      \"description\": \"Kustomize-specific source configuration.\",\n      \"properties\": {\n        \"namePrefix\": {\n          \"type\": \"string\",\n          \"description\": \"Prefix to append to all resource names.\"\n        },\n        \"nameSuffix\": {\n          \"type\": \"string\",\n          \"\
  description\": \"Suffix to append to all resource names.\"\n        },\n        \"images\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"List of image overrides in name=tag format.\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"repoURL\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-application-source-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: ApplicationSource
---
