---
description: RebootWorkspacesResult schema from Amazon WorkSpaces API
layout: schema
name: RebootWorkspacesResult
properties_list:
- description: ''
  name: FailedRequests
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-reboot-workspaces-result-schema.json
slug: workspaces-reboot-workspaces-result
source_filename: workspaces-reboot-workspaces-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailedRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailedRebootWorkspaceRequests\"\n        },\n        {\n          \"description\": \"Information about the WorkSpaces that could not be rebooted.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RebootWorkspacesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-reboot-workspaces-result-schema.json\",\n  \"description\": \"RebootWorkspacesResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-reboot-workspaces-result-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: RebootWorkspacesResult
---
