---
description: CreateUpdatedWorkspaceImageResult schema from Amazon WorkSpaces API
layout: schema
name: CreateUpdatedWorkspaceImageResult
properties_list:
- description: ''
  name: ImageId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-create-updated-workspace-image-result-schema.json
slug: workspaces-create-updated-workspace-image-result
source_filename: workspaces-create-updated-workspace-image-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageId\"\n        },\n        {\n          \"description\": \"The identifier of the new updated WorkSpace image.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateUpdatedWorkspaceImageResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-updated-workspace-image-result-schema.json\",\n  \"description\": \"CreateUpdatedWorkspaceImageResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-updated-workspace-image-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateUpdatedWorkspaceImageResult
---
