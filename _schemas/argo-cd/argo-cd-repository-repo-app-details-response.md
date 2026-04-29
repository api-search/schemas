---
description: repositoryRepoAppDetailsResponse schema from Argo CD API
layout: schema
name: repositoryRepoAppDetailsResponse
properties_list:
- description: ''
  name: directory
  type: object
- description: ''
  name: helm
  type: object
- description: ''
  name: kustomize
  type: object
- description: ''
  name: plugin
  type: object
- description: ''
  name: type
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-repository-repo-app-details-response-schema.json
slug: argo-cd-repository-repo-app-details-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-repo-app-details-response-schema.json\",\n  \"title\": \"repositoryRepoAppDetailsResponse\",\n  \"description\": \"repositoryRepoAppDetailsResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"directory\": {\n      \"$ref\": \"#/definitions/repositoryDirectoryAppSpec\"\n    },\n    \"helm\": {\n      \"$ref\": \"#/definitions/repositoryHelmAppSpec\"\n    },\n    \"kustomize\": {\n      \"$ref\": \"#/definitions/repositoryKustomizeAppSpec\"\n    },\n    \"plugin\": {\n      \"$ref\": \"#/definitions/repositoryPluginAppSpec\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-repo-app-details-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: repositoryRepoAppDetailsResponse
---
