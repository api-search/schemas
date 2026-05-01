---
description: Represents a summary of the properties of a workspace.
layout: schema
name: WorkspaceSummary
properties_list:
- description: ''
  name: workspaceId
  type: object
- description: ''
  name: alias
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-workspace-summary-schema.json
slug: amazon-managed-prometheus-workspace-summary
source_filename: amazon-managed-prometheus-workspace-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-workspace-summary-schema.json\",\n  \"title\": \"WorkspaceSummary\",\n  \"description\": \"Represents a summary of the properties of a workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"Unique string identifying this workspace.\"\n        }\n      ]\n    },\n    \"alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceAlias\"\n        },\n        {\n          \"description\": \"Alias of this workspace.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceArn\"\n        },\n      \
  \  {\n          \"description\": \"The AmazonResourceName of this workspace.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceStatus\"\n        },\n        {\n          \"description\": \"The status of this workspace.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the workspace was created.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags of this workspace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"workspaceId\",\n    \"arn\",\n    \"status\",\n    \"createdAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-workspace-summary-schema.json
tags:
- Containers
- Monitoring
- Observability
- Prometheus
title: WorkspaceSummary
---
