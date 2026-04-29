---
description: RebuildWorkspacesRequest schema from Amazon WorkSpaces API
layout: schema
name: RebuildWorkspacesRequest
properties_list:
- description: ''
  name: RebuildWorkspaceRequests
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-rebuild-workspaces-request-schema.json
slug: workspaces-rebuild-workspaces-request
source_filename: workspaces-rebuild-workspaces-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"RebuildWorkspaceRequests\"\n  ],\n  \"title\": \"RebuildWorkspacesRequest\",\n  \"properties\": {\n    \"RebuildWorkspaceRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RebuildWorkspaceRequests\"\n        },\n        {\n          \"description\": \"The WorkSpace to rebuild. You can specify a single WorkSpace.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-rebuild-workspaces-request-schema.json\",\n  \"description\": \"RebuildWorkspacesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-rebuild-workspaces-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: RebuildWorkspacesRequest
---
