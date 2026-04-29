---
description: ModifyWorkspacePropertiesRequest schema from Amazon WorkSpaces API
layout: schema
name: ModifyWorkspacePropertiesRequest
properties_list:
- description: ''
  name: WorkspaceId
  type: object
- description: ''
  name: WorkspaceProperties
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-modify-workspace-properties-request-schema.json
slug: workspaces-modify-workspace-properties-request
source_filename: workspaces-modify-workspace-properties-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"WorkspaceId\",\n    \"WorkspaceProperties\"\n  ],\n  \"title\": \"ModifyWorkspacePropertiesRequest\",\n  \"properties\": {\n    \"WorkspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The identifier of the WorkSpace.\"\n        }\n      ]\n    },\n    \"WorkspaceProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceProperties\"\n        },\n        {\n          \"description\": \"The properties of the WorkSpace.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-workspace-properties-request-schema.json\",\n  \"description\": \"ModifyWorkspacePropertiesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-workspace-properties-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ModifyWorkspacePropertiesRequest
---
