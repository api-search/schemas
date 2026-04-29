---
description: CreateWorkspaceApiKeyRequest schema from Amazon Managed Grafana API
layout: schema
name: CreateWorkspaceApiKeyRequest
properties_list:
- description: ''
  name: keyName
  type: object
- description: ''
  name: keyRole
  type: object
- description: ''
  name: secondsToLive
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-create-workspace-api-key-request-schema.json
slug: amazon-managed-grafana-create-workspace-api-key-request
source_filename: amazon-managed-grafana-create-workspace-api-key-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-create-workspace-api-key-request-schema.json\",\n  \"title\": \"CreateWorkspaceApiKeyRequest\",\n  \"description\": \"CreateWorkspaceApiKeyRequest schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApiKeyName\"\n        },\n        {\n          \"description\": \"Specifies the name of the key. Keynames must be unique to the workspace.\"\n        }\n      ]\n    },\n    \"keyRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Specifies the permission level of the key.</p> <p> Valid values: <code>VIEWER</code>|<code>EDITOR</code>|<code>ADMIN</code>\
  \ </p>\"\n        }\n      ]\n    },\n    \"secondsToLive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateWorkspaceApiKeyRequestSecondsToLiveInteger\"\n        },\n        {\n          \"description\": \"Specifies the time in seconds until the key expires. Keys can be valid for up to 30 days.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"keyName\",\n    \"keyRole\",\n    \"secondsToLive\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-create-workspace-api-key-request-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: CreateWorkspaceApiKeyRequest
---
