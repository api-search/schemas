---
description: The conflict resolution policy.
layout: schema
name: ConflictResolutionPolicy
properties_list:
- description: The conflict resolution mode.
  name: mode
  type: string
- description: The path for the last-writer-wins conflict resolution.
  name: conflictResolutionPath
  type: string
- description: The stored procedure for custom conflict resolution.
  name: conflictResolutionProcedure
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-conflict-resolution-policy-schema.json
slug: azure-cosmos-db-conflict-resolution-policy
source_filename: azure-cosmos-db-conflict-resolution-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConflictResolutionPolicy\",\n  \"type\": \"object\",\n  \"description\": \"The conflict resolution policy.\",\n  \"properties\": {\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"The conflict resolution mode.\"\n    },\n    \"conflictResolutionPath\": {\n      \"type\": \"string\",\n      \"description\": \"The path for the last-writer-wins conflict resolution.\"\n    },\n    \"conflictResolutionProcedure\": {\n      \"type\": \"string\",\n      \"description\": \"The stored procedure for custom conflict resolution.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-conflict-resolution-policy-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ConflictResolutionPolicy
---
