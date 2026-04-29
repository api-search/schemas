---
description: MigrateWorkspaceRequest schema from Amazon WorkSpaces API
layout: schema
name: MigrateWorkspaceRequest
properties_list:
- description: ''
  name: SourceWorkspaceId
  type: object
- description: ''
  name: BundleId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-migrate-workspace-request-schema.json
slug: workspaces-migrate-workspace-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"SourceWorkspaceId\",\n    \"BundleId\"\n  ],\n  \"title\": \"MigrateWorkspaceRequest\",\n  \"properties\": {\n    \"SourceWorkspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The identifier of the WorkSpace to migrate from.\"\n        }\n      ]\n    },\n    \"BundleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BundleId\"\n        },\n        {\n          \"description\": \"The identifier of the target bundle type to migrate the WorkSpace to.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-migrate-workspace-request-schema.json\",\n  \"description\": \"MigrateWorkspaceRequest schema from Amazon WorkSpaces API\"\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-migrate-workspace-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: MigrateWorkspaceRequest
---
