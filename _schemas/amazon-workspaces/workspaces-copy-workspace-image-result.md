---
description: CopyWorkspaceImageResult schema from Amazon WorkSpaces API
layout: schema
name: CopyWorkspaceImageResult
properties_list:
- description: ''
  name: ImageId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-copy-workspace-image-result-schema.json
slug: workspaces-copy-workspace-image-result
source_filename: workspaces-copy-workspace-image-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageId\"\n        },\n        {\n          \"description\": \"The identifier of the image.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CopyWorkspaceImageResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-copy-workspace-image-result-schema.json\",\n  \"description\": \"CopyWorkspaceImageResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-copy-workspace-image-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CopyWorkspaceImageResult
---
