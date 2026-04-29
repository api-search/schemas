---
description: Represents the health status of the Connect server and its dependencies.
layout: schema
name: ServerHealth
properties_list:
- description: The name of the Connect server.
  name: name
  type: string
- description: The version of the Connect server.
  name: version
  type: string
- description: The health status of server dependencies.
  name: dependencies
  type: array
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-connect-server-health-schema.json
slug: 1password-connect-server-health
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-server-health-schema.json\",\n  \"title\": \"ServerHealth\",\n  \"description\": \"Represents the health status of the Connect server and its dependencies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Connect server.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the Connect server.\"\n    },\n    \"dependencies\": {\n      \"type\": \"array\",\n      \"description\": \"The health status of server dependencies.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"service\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the dependency service.\"\n          },\n          \"status\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"The status of the dependency.\",\n            \"enum\": [\n              \"ACTIVE\",\n              \"INACTIVE\",\n              \"ERROR\"\n            ]\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Additional information about the dependency status.\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-server-health-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: ServerHealth
---
