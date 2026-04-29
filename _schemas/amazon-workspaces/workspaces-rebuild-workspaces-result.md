---
description: RebuildWorkspacesResult schema from Amazon WorkSpaces API
layout: schema
name: RebuildWorkspacesResult
properties_list:
- description: ''
  name: FailedRequests
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-rebuild-workspaces-result-schema.json
slug: workspaces-rebuild-workspaces-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailedRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailedRebuildWorkspaceRequests\"\n        },\n        {\n          \"description\": \"Information about the WorkSpace that could not be rebuilt.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RebuildWorkspacesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-rebuild-workspaces-result-schema.json\",\n  \"description\": \"RebuildWorkspacesResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-rebuild-workspaces-result-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: RebuildWorkspacesResult
---
