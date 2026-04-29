---
description: ''
layout: schema
name: User
properties_list:
- description: ''
  name: userId
  type: string
- description: ''
  name: username
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: organizationId
  type: string
provider_name: Spot
provider_slug: spot
schema_file: json-schema/spot-administration-user-schema.json
slug: spot-administration-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\"\n    },\n    \"username\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"organizationId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/spot-administration-user-schema.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: User
---
