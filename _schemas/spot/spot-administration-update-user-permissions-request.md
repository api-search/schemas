---
description: ''
layout: schema
name: UpdateUserPermissionsRequest
properties_list:
- description: ''
  name: role
  type: string
- description: ''
  name: accounts
  type: array
provider_name: Spot
provider_slug: spot
schema_file: json-schema/spot-administration-update-user-permissions-request-schema.json
slug: spot-administration-update-user-permissions-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateUserPermissionsRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"role\": {\n      \"type\": \"string\"\n    },\n    \"accounts\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/spot-administration-update-user-permissions-request-schema.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: UpdateUserPermissionsRequest
---
