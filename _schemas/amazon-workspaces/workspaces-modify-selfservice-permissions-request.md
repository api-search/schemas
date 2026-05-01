---
description: ModifySelfservicePermissionsRequest schema from Amazon WorkSpaces API
layout: schema
name: ModifySelfservicePermissionsRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: SelfservicePermissions
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-modify-selfservice-permissions-request-schema.json
slug: workspaces-modify-selfservice-permissions-request
source_filename: workspaces-modify-selfservice-permissions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceId\",\n    \"SelfservicePermissions\"\n  ],\n  \"title\": \"ModifySelfservicePermissionsRequest\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The identifier of the directory.\"\n        }\n      ]\n    },\n    \"SelfservicePermissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SelfservicePermissions\"\n        },\n        {\n          \"description\": \"The permissions to enable or disable self-service capabilities.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-selfservice-permissions-request-schema.json\",\n  \"description\": \"ModifySelfservicePermissionsRequest\
  \ schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-selfservice-permissions-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ModifySelfservicePermissionsRequest
---
