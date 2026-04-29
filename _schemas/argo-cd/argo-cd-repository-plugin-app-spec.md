---
description: repositoryPluginAppSpec schema from Argo CD API
layout: schema
name: repositoryPluginAppSpec
properties_list:
- description: ''
  name: parametersAnnouncement
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-repository-plugin-app-spec-schema.json
slug: argo-cd-repository-plugin-app-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-plugin-app-spec-schema.json\",\n  \"title\": \"repositoryPluginAppSpec\",\n  \"description\": \"repositoryPluginAppSpec schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parametersAnnouncement\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/repositoryParameterAnnouncement\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-plugin-app-spec-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: repositoryPluginAppSpec
---
