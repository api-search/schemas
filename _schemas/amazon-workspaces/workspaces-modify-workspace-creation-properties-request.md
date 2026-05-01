---
description: ModifyWorkspaceCreationPropertiesRequest schema from Amazon WorkSpaces API
layout: schema
name: ModifyWorkspaceCreationPropertiesRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: WorkspaceCreationProperties
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-modify-workspace-creation-properties-request-schema.json
slug: workspaces-modify-workspace-creation-properties-request
source_filename: workspaces-modify-workspace-creation-properties-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceId\",\n    \"WorkspaceCreationProperties\"\n  ],\n  \"title\": \"ModifyWorkspaceCreationPropertiesRequest\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The identifier of the directory.\"\n        }\n      ]\n    },\n    \"WorkspaceCreationProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceCreationProperties\"\n        },\n        {\n          \"description\": \"The default properties for creating WorkSpaces.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-workspace-creation-properties-request-schema.json\",\n  \"description\": \"ModifyWorkspaceCreationPropertiesRequest\
  \ schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-workspace-creation-properties-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ModifyWorkspaceCreationPropertiesRequest
---
