---
description: CreateUpdatedWorkspaceImageRequest schema from Amazon WorkSpaces API
layout: schema
name: CreateUpdatedWorkspaceImageRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: SourceImageId
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-create-updated-workspace-image-request-schema.json
slug: workspaces-create-updated-workspace-image-request
source_filename: workspaces-create-updated-workspace-image-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"Name\",\n    \"Description\",\n    \"SourceImageId\"\n  ],\n  \"title\": \"CreateUpdatedWorkspaceImageRequest\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageName\"\n        },\n        {\n          \"description\": \"The name of the new updated WorkSpace image.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageDescription\"\n        },\n        {\n          \"description\": \"A description of whether updates for the WorkSpace image are available.\"\n        }\n      ]\n    },\n    \"SourceImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageId\"\n        },\n        {\n          \"description\": \"The identifier of the source WorkSpace image.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>The tags that you want to add to the new updated WorkSpace image.</p> <note> <p>To add tags at the same time when you're creating the updated image, you must create an IAM policy that grants your IAM user permissions to use <code>workspaces:CreateTags</code>. </p> </note>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-updated-workspace-image-request-schema.json\",\n  \"description\": \"CreateUpdatedWorkspaceImageRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-updated-workspace-image-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateUpdatedWorkspaceImageRequest
---
