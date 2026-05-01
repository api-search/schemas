---
description: RebootWorkspacesRequest schema from Amazon WorkSpaces API
layout: schema
name: RebootWorkspacesRequest
properties_list:
- description: ''
  name: RebootWorkspaceRequests
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-reboot-workspaces-request-schema.json
slug: workspaces-reboot-workspaces-request
source_filename: workspaces-reboot-workspaces-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"RebootWorkspaceRequests\"\n  ],\n  \"title\": \"RebootWorkspacesRequest\",\n  \"properties\": {\n    \"RebootWorkspaceRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RebootWorkspaceRequests\"\n        },\n        {\n          \"description\": \"The WorkSpaces to reboot. You can specify up to 25 WorkSpaces.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-reboot-workspaces-request-schema.json\",\n  \"description\": \"RebootWorkspacesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-reboot-workspaces-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: RebootWorkspacesRequest
---
