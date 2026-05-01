---
description: MigrateWorkspaceResult schema from Amazon WorkSpaces API
layout: schema
name: MigrateWorkspaceResult
properties_list:
- description: ''
  name: SourceWorkspaceId
  type: object
- description: ''
  name: TargetWorkspaceId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-migrate-workspace-result-schema.json
slug: workspaces-migrate-workspace-result
source_filename: workspaces-migrate-workspace-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceWorkspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The original identifier of the WorkSpace that is being migrated.\"\n        }\n      ]\n    },\n    \"TargetWorkspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The new identifier of the WorkSpace that is being migrated. If the migration does not succeed, the target WorkSpace ID will not be used, and the WorkSpace will still have the original WorkSpace ID.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MigrateWorkspaceResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-migrate-workspace-result-schema.json\",\n\
  \  \"description\": \"MigrateWorkspaceResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-migrate-workspace-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: MigrateWorkspaceResult
---
