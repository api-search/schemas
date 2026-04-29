---
description: CreateWorkspaceImageRequest schema from Amazon WorkSpaces API
layout: schema
name: CreateWorkspaceImageRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: WorkspaceId
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-create-workspace-image-request-schema.json
slug: workspaces-create-workspace-image-request
source_filename: workspaces-create-workspace-image-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"Name\",\n    \"Description\",\n    \"WorkspaceId\"\n  ],\n  \"title\": \"CreateWorkspaceImageRequest\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageName\"\n        },\n        {\n          \"description\": \"The name of the new WorkSpace image.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageDescription\"\n        },\n        {\n          \"description\": \"The description of the new WorkSpace image.\"\n        }\n      ]\n    },\n    \"WorkspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The identifier of the source WorkSpace\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\
  \n        },\n        {\n          \"description\": \"The tags that you want to add to the new WorkSpace image. To add tags when you're creating the image, you must create an IAM policy that grants your IAM user permission to use <code>workspaces:CreateTags</code>.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-workspace-image-request-schema.json\",\n  \"description\": \"CreateWorkspaceImageRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-workspace-image-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateWorkspaceImageRequest
---
