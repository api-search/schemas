---
description: Represents the input of a CreateWorkspace operation.
layout: schema
name: CreateWorkspaceRequest
properties_list:
- description: ''
  name: alias
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-create-workspace-request-schema.json
slug: amazon-managed-prometheus-create-workspace-request
source_filename: amazon-managed-prometheus-create-workspace-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-workspace-request-schema.json\",\n  \"title\": \"CreateWorkspaceRequest\",\n  \"description\": \"Represents the input of a CreateWorkspace operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceAlias\"\n        },\n        {\n          \"description\": \"An optional user-assigned alias for this workspace. This alias is for user reference and does not need to be unique.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyToken\"\n        },\n        {\n          \"description\": \"Optional, unique, case-sensitive, user-provided identifier to ensure the idempotency of the\
  \ request.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Optional, user-provided tags for this workspace.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-workspace-request-schema.json
tags:
- Containers
- Monitoring
- Observability
- Prometheus
title: CreateWorkspaceRequest
---
