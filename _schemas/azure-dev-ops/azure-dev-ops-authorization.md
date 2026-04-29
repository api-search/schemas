---
description: Authorization info used to access a resource (like code repository).
layout: schema
name: Authorization
properties_list:
- description: Type of authorization.
  name: authorizationType
  type: string
- description: Authorization parameters corresponding to the authorization type.
  name: parameters
  type: object
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-authorization-schema.json
slug: azure-dev-ops-authorization
source_filename: azure-dev-ops-authorization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-authorization-schema.json\",\n  \"title\": \"Authorization\",\n  \"description\": \"Authorization info used to access a resource (like code repository).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorizationType\": {\n      \"description\": \"Type of authorization.\",\n      \"enum\": [\n        \"personalAccessToken\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"AuthorizationType\"\n      }\n    },\n    \"parameters\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Authorization parameters corresponding to the authorization type.\",\n      \"type\": \"object\"\n    }\n  },\n  \"required\": [\n    \"authorizationType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-authorization-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: Authorization
---
