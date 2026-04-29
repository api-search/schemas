---
description: repositoryManifestResponse schema from Argo CD API
layout: schema
name: repositoryManifestResponse
properties_list:
- description: ''
  name: commands
  type: array
- description: ''
  name: manifests
  type: array
- description: ''
  name: namespace
  type: string
- description: ''
  name: revision
  type: string
- description: ''
  name: server
  type: string
- description: ''
  name: sourceType
  type: string
- description: ''
  name: verifyResult
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-repository-manifest-response-schema.json
slug: argo-cd-repository-manifest-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-manifest-response-schema.json\",\n  \"title\": \"repositoryManifestResponse\",\n  \"description\": \"repositoryManifestResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"commands\": {\n      \"type\": \"array\",\n      \"title\": \"Commands is the list of commands used to hydrate the manifests\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"manifests\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"revision\": {\n      \"type\": \"string\",\n      \"title\": \"resolved revision\"\n    },\n    \"server\": {\n      \"type\": \"string\"\n    },\n    \"sourceType\": {\n      \"type\": \"string\"\n    },\n    \"verifyResult\"\
  : {\n      \"type\": \"string\",\n      \"title\": \"Raw response of git verify-commit operation (always the empty string for Helm)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-manifest-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: repositoryManifestResponse
---
