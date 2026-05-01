---
description: Describes the connection status of a WorkSpace.
layout: schema
name: WorkspaceConnectionStatus
properties_list:
- description: ''
  name: WorkspaceId
  type: object
- description: ''
  name: ConnectionState
  type: object
- description: ''
  name: ConnectionStateCheckTimestamp
  type: object
- description: ''
  name: LastKnownUserConnectionTimestamp
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-workspace-connection-status-schema.json
slug: workspaces-workspace-connection-status
source_filename: workspaces-workspace-connection-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The identifier of the WorkSpace.\"\n        }\n      ]\n    },\n    \"ConnectionState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionState\"\n        },\n        {\n          \"description\": \"The connection state of the WorkSpace. The connection state is unknown if the WorkSpace is stopped.\"\n        }\n      ]\n    },\n    \"ConnectionStateCheckTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp of the connection status check.\"\n        }\n      ]\n    },\n    \"LastKnownUserConnectionTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n   \
  \     {\n          \"description\": \"The timestamp of the last known user connection.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the connection status of a WorkSpace.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkspaceConnectionStatus\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-connection-status-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-connection-status-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: WorkspaceConnectionStatus
---
