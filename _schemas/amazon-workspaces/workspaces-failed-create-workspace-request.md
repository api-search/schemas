---
description: Describes a WorkSpace that cannot be created.
layout: schema
name: FailedCreateWorkspaceRequest
properties_list:
- description: ''
  name: WorkspaceRequest
  type: object
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: ErrorMessage
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-failed-create-workspace-request-schema.json
slug: workspaces-failed-create-workspace-request
source_filename: workspaces-failed-create-workspace-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkspaceRequest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceRequest\"\n        },\n        {\n          \"description\": \"Information about the WorkSpace.\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorType\"\n        },\n        {\n          \"description\": \"The error code that is returned if the WorkSpace cannot be created.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The text of the error message that is returned if the WorkSpace cannot be created.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes a WorkSpace that cannot be created.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FailedCreateWorkspaceRequest\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-failed-create-workspace-request-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-failed-create-workspace-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: FailedCreateWorkspaceRequest
---
