---
description: ModifyWorkspaceStateRequest schema from Amazon WorkSpaces API
layout: schema
name: ModifyWorkspaceStateRequest
properties_list:
- description: ''
  name: WorkspaceId
  type: object
- description: ''
  name: WorkspaceState
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-modify-workspace-state-request-schema.json
slug: workspaces-modify-workspace-state-request
source_filename: workspaces-modify-workspace-state-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"WorkspaceId\",\n    \"WorkspaceState\"\n  ],\n  \"title\": \"ModifyWorkspaceStateRequest\",\n  \"properties\": {\n    \"WorkspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The identifier of the WorkSpace.\"\n        }\n      ]\n    },\n    \"WorkspaceState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetWorkspaceState\"\n        },\n        {\n          \"description\": \"The WorkSpace state.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-workspace-state-request-schema.json\",\n  \"description\": \"ModifyWorkspaceStateRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-workspace-state-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ModifyWorkspaceStateRequest
---
