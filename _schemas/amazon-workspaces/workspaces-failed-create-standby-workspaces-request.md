---
description: Describes the standby WorkSpace that could not be created.
layout: schema
name: FailedCreateStandbyWorkspacesRequest
properties_list:
- description: ''
  name: StandbyWorkspaceRequest
  type: object
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: ErrorMessage
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-failed-create-standby-workspaces-request-schema.json
slug: workspaces-failed-create-standby-workspaces-request
source_filename: workspaces-failed-create-standby-workspaces-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"StandbyWorkspaceRequest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StandbyWorkspace\"\n        },\n        {\n          \"description\": \"Information about the standby WorkSpace that could not be created.\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceErrorCode\"\n        },\n        {\n          \"description\": \"The error code that is returned if the standby WorkSpace could not be created.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The text of the error message that is returned if the standby WorkSpace could not be created.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the standby WorkSpace that could not be created.\",\n\
  \  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FailedCreateStandbyWorkspacesRequest\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-failed-create-standby-workspaces-request-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-failed-create-standby-workspaces-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: FailedCreateStandbyWorkspacesRequest
---
