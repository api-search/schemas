---
description: ''
layout: schema
name: CreateProgrammaticUserRequest
properties_list:
- description: Name of the programmatic user.
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: accounts
  type: array
provider_name: Spot
provider_slug: spot
schema_file: json-schema/spot-administration-create-programmatic-user-request-schema.json
slug: spot-administration-create-programmatic-user-request
source_filename: spot-administration-create-programmatic-user-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateProgrammaticUserRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the programmatic user.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"accounts\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/spot-administration-create-programmatic-user-request-schema.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: CreateProgrammaticUserRequest
---
