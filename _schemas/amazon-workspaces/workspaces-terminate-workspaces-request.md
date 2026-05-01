---
description: TerminateWorkspacesRequest schema from Amazon WorkSpaces API
layout: schema
name: TerminateWorkspacesRequest
properties_list:
- description: ''
  name: TerminateWorkspaceRequests
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-terminate-workspaces-request-schema.json
slug: workspaces-terminate-workspaces-request
source_filename: workspaces-terminate-workspaces-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"TerminateWorkspaceRequests\"\n  ],\n  \"title\": \"TerminateWorkspacesRequest\",\n  \"properties\": {\n    \"TerminateWorkspaceRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TerminateWorkspaceRequests\"\n        },\n        {\n          \"description\": \"The WorkSpaces to terminate. You can specify up to 25 WorkSpaces.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-terminate-workspaces-request-schema.json\",\n  \"description\": \"TerminateWorkspacesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-terminate-workspaces-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: TerminateWorkspacesRequest
---
