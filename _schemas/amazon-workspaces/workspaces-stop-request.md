---
description: Describes the information used to stop a WorkSpace.
layout: schema
name: StopRequest
properties_list:
- description: ''
  name: WorkspaceId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-stop-request-schema.json
slug: workspaces-stop-request
source_filename: workspaces-stop-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The identifier of the WorkSpace.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the information used to stop a WorkSpace.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StopRequest\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-stop-request-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-stop-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: StopRequest
---
