---
description: ProjectCreateRequest defines project creation parameters.
layout: schema
name: projectProjectCreateRequest
properties_list:
- description: ''
  name: project
  type: object
- description: ''
  name: upsert
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-project-project-create-request-schema.json
slug: argo-cd-project-project-create-request
source_filename: argo-cd-project-project-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-project-project-create-request-schema.json\",\n  \"title\": \"projectProjectCreateRequest\",\n  \"description\": \"ProjectCreateRequest defines project creation parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"project\": {\n      \"$ref\": \"#/definitions/v1alpha1AppProject\"\n    },\n    \"upsert\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-project-project-create-request-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: projectProjectCreateRequest
---
