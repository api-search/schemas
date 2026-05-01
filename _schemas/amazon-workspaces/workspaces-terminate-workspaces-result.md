---
description: TerminateWorkspacesResult schema from Amazon WorkSpaces API
layout: schema
name: TerminateWorkspacesResult
properties_list:
- description: ''
  name: FailedRequests
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-terminate-workspaces-result-schema.json
slug: workspaces-terminate-workspaces-result
source_filename: workspaces-terminate-workspaces-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailedRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailedTerminateWorkspaceRequests\"\n        },\n        {\n          \"description\": \"Information about the WorkSpaces that could not be terminated.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TerminateWorkspacesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-terminate-workspaces-result-schema.json\",\n  \"description\": \"TerminateWorkspacesResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-terminate-workspaces-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: TerminateWorkspacesResult
---
