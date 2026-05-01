---
description: CopyWorkspaceImageRequest schema from Amazon WorkSpaces API
layout: schema
name: CopyWorkspaceImageRequest
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
  name: SourceRegion
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-copy-workspace-image-request-schema.json
slug: workspaces-copy-workspace-image-request
source_filename: workspaces-copy-workspace-image-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"Name\",\n    \"SourceImageId\",\n    \"SourceRegion\"\n  ],\n  \"title\": \"CopyWorkspaceImageRequest\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageName\"\n        },\n        {\n          \"description\": \"The name of the image.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageDescription\"\n        },\n        {\n          \"description\": \"A description of the image.\"\n        }\n      ]\n    },\n    \"SourceImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageId\"\n        },\n        {\n          \"description\": \"The identifier of the source image.\"\n        }\n      ]\n    },\n    \"SourceRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Region\"\n  \
  \      },\n        {\n          \"description\": \"The identifier of the source Region.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags for the image.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-copy-workspace-image-request-schema.json\",\n  \"description\": \"CopyWorkspaceImageRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-copy-workspace-image-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CopyWorkspaceImageRequest
---
