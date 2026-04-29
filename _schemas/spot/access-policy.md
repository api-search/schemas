---
description: A Spot access policy defines a set of permissions that control what actions users and groups can perform on Spot platform services and resources.
layout: schema
name: Spot Access Policy
properties_list:
- description: The unique identifier of the access policy.
  name: id
  type: string
- description: The name of the access policy.
  name: name
  type: string
- description: A description of the access policy.
  name: description
  type: string
- description: The list of permissions granted by this policy.
  name: permissions
  type: array
provider_name: Spot
provider_slug: spot
schema_file: json-schema/access-policy.json
slug: access-policy
source_filename: access-policy.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/spot/blob/main/json-schema/access-policy.json\",\n  \"title\": \"Spot Access Policy\",\n  \"description\": \"A Spot access policy defines a set of permissions that control what actions users and groups can perform on Spot platform services and resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the access policy.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the access policy.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the access policy.\"\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"serviceId\": {\n            \"type\": \"string\",\n           \
  \ \"description\": \"The Spot service identifier the permission applies to.\"\n          },\n          \"actions\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"The list of permitted actions on the service.\"\n          }\n        }\n      },\n      \"description\": \"The list of permissions granted by this policy.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/access-policy.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: Spot Access Policy
---
