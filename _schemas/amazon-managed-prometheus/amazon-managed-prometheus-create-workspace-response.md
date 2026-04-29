---
description: Represents the output of a CreateWorkspace operation.
layout: schema
name: CreateWorkspaceResponse
properties_list:
- description: ''
  name: workspaceId
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-create-workspace-response-schema.json
slug: amazon-managed-prometheus-create-workspace-response
source_filename: amazon-managed-prometheus-create-workspace-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-workspace-response-schema.json\",\n  \"title\": \"CreateWorkspaceResponse\",\n  \"description\": \"Represents the output of a CreateWorkspace operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The generated ID of the workspace that was just created.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceArn\"\n        },\n        {\n          \"description\": \"The ARN of the workspace that was just created.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceStatus\"\
  \n        },\n        {\n          \"description\": \"The status of the workspace that was just created (usually CREATING).\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags of this workspace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"workspaceId\",\n    \"arn\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-workspace-response-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: CreateWorkspaceResponse
---
