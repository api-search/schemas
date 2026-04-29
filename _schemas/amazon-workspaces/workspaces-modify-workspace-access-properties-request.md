---
description: ModifyWorkspaceAccessPropertiesRequest schema from Amazon WorkSpaces API
layout: schema
name: ModifyWorkspaceAccessPropertiesRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: WorkspaceAccessProperties
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-modify-workspace-access-properties-request-schema.json
slug: workspaces-modify-workspace-access-properties-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceId\",\n    \"WorkspaceAccessProperties\"\n  ],\n  \"title\": \"ModifyWorkspaceAccessPropertiesRequest\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The identifier of the directory.\"\n        }\n      ]\n    },\n    \"WorkspaceAccessProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceAccessProperties\"\n        },\n        {\n          \"description\": \"The device types and operating systems to enable or disable for access.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-workspace-access-properties-request-schema.json\",\n  \"description\": \"ModifyWorkspaceAccessPropertiesRequest\
  \ schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-workspace-access-properties-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ModifyWorkspaceAccessPropertiesRequest
---
