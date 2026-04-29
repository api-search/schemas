---
description: DeleteWorkspaceApiKeyResponse schema from Amazon Managed Grafana API
layout: schema
name: DeleteWorkspaceApiKeyResponse
properties_list:
- description: ''
  name: keyName
  type: object
- description: ''
  name: workspaceId
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-delete-workspace-api-key-response-schema.json
slug: amazon-managed-grafana-delete-workspace-api-key-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-delete-workspace-api-key-response-schema.json\",\n  \"title\": \"DeleteWorkspaceApiKeyResponse\",\n  \"description\": \"DeleteWorkspaceApiKeyResponse schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApiKeyName\"\n        },\n        {\n          \"description\": \"The name of the key that was deleted.\"\n        }\n      ]\n    },\n    \"workspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The ID of the workspace where the key was deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"keyName\",\n    \"workspaceId\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-delete-workspace-api-key-response-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: DeleteWorkspaceApiKeyResponse
---
