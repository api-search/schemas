---
description: CreateStandbyWorkspacesResult schema from Amazon WorkSpaces API
layout: schema
name: CreateStandbyWorkspacesResult
properties_list:
- description: ''
  name: FailedStandbyRequests
  type: object
- description: ''
  name: PendingStandbyRequests
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-create-standby-workspaces-result-schema.json
slug: workspaces-create-standby-workspaces-result
source_filename: workspaces-create-standby-workspaces-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailedStandbyRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailedCreateStandbyWorkspacesRequestList\"\n        },\n        {\n          \"description\": \"Information about the standby WorkSpace that could not be created. \"\n        }\n      ]\n    },\n    \"PendingStandbyRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PendingCreateStandbyWorkspacesRequestList\"\n        },\n        {\n          \"description\": \"Information about the standby WorkSpace that was created.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateStandbyWorkspacesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-standby-workspaces-result-schema.json\",\n  \"description\": \"CreateStandbyWorkspacesResult schema\
  \ from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-standby-workspaces-result-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateStandbyWorkspacesResult
---
