---
description: A list of Argo CD applications.
layout: schema
name: ApplicationList
properties_list:
- description: Array of application objects.
  name: items
  type: array
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-application-list-schema.json
slug: argo-cd-application-list
source_filename: argo-cd-application-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-application-list-schema.json\",\n  \"title\": \"ApplicationList\",\n  \"description\": \"A list of Argo CD applications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Array of application objects.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Application\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-application-list-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: ApplicationList
---
