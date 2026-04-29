---
description: ProjectTokenCreateRequest defines project token creation parameters.
layout: schema
name: projectProjectTokenCreateRequest
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: expiresIn
  type: integer
- description: ''
  name: id
  type: string
- description: ''
  name: project
  type: string
- description: ''
  name: role
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-project-project-token-create-request-schema.json
slug: argo-cd-project-project-token-create-request
source_filename: argo-cd-project-project-token-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-project-project-token-create-request-schema.json\",\n  \"title\": \"projectProjectTokenCreateRequest\",\n  \"description\": \"ProjectTokenCreateRequest defines project token creation parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"expiresIn\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"expiresIn represents a duration in seconds\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"project\": {\n      \"type\": \"string\"\n    },\n    \"role\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-project-project-token-create-request-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: projectProjectTokenCreateRequest
---
