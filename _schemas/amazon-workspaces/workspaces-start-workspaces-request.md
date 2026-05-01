---
description: StartWorkspacesRequest schema from Amazon WorkSpaces API
layout: schema
name: StartWorkspacesRequest
properties_list:
- description: ''
  name: StartWorkspaceRequests
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-start-workspaces-request-schema.json
slug: workspaces-start-workspaces-request
source_filename: workspaces-start-workspaces-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"StartWorkspaceRequests\"\n  ],\n  \"title\": \"StartWorkspacesRequest\",\n  \"properties\": {\n    \"StartWorkspaceRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartWorkspaceRequests\"\n        },\n        {\n          \"description\": \"The WorkSpaces to start. You can specify up to 25 WorkSpaces.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-start-workspaces-request-schema.json\",\n  \"description\": \"StartWorkspacesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-start-workspaces-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: StartWorkspacesRequest
---
