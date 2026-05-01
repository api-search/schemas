---
description: StopWorkspacesRequest schema from Amazon WorkSpaces API
layout: schema
name: StopWorkspacesRequest
properties_list:
- description: ''
  name: StopWorkspaceRequests
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-stop-workspaces-request-schema.json
slug: workspaces-stop-workspaces-request
source_filename: workspaces-stop-workspaces-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"StopWorkspaceRequests\"\n  ],\n  \"title\": \"StopWorkspacesRequest\",\n  \"properties\": {\n    \"StopWorkspaceRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StopWorkspaceRequests\"\n        },\n        {\n          \"description\": \"The WorkSpaces to stop. You can specify up to 25 WorkSpaces.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-stop-workspaces-request-schema.json\",\n  \"description\": \"StopWorkspacesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-stop-workspaces-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: StopWorkspacesRequest
---
