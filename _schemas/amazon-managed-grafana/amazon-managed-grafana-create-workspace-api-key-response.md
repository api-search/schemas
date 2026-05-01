---
description: CreateWorkspaceApiKeyResponse schema from Amazon Managed Grafana API
layout: schema
name: CreateWorkspaceApiKeyResponse
properties_list:
- description: ''
  name: key
  type: object
- description: ''
  name: keyName
  type: object
- description: ''
  name: workspaceId
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-create-workspace-api-key-response-schema.json
slug: amazon-managed-grafana-create-workspace-api-key-response
source_filename: amazon-managed-grafana-create-workspace-api-key-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-create-workspace-api-key-response-schema.json\",\n  \"title\": \"CreateWorkspaceApiKeyResponse\",\n  \"description\": \"CreateWorkspaceApiKeyResponse schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApiKeyToken\"\n        },\n        {\n          \"description\": \"The key token. Use this value as a bearer token to authenticate HTTP requests to the workspace.\"\n        }\n      ]\n    },\n    \"keyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApiKeyName\"\n        },\n        {\n          \"description\": \"The name of the key that was created.\"\n        }\n      ]\n    },\n    \"workspaceId\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The ID of the workspace that the key is valid for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"keyName\",\n    \"workspaceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-create-workspace-api-key-response-schema.json
tags:
- Dashboards
- Monitoring
- Observability
- Visualization
title: CreateWorkspaceApiKeyResponse
---
