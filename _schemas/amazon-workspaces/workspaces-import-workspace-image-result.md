---
description: ImportWorkspaceImageResult schema from Amazon WorkSpaces API
layout: schema
name: ImportWorkspaceImageResult
properties_list:
- description: ''
  name: ImageId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-import-workspace-image-result-schema.json
slug: workspaces-import-workspace-image-result
source_filename: workspaces-import-workspace-image-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageId\"\n        },\n        {\n          \"description\": \"The identifier of the WorkSpace image.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImportWorkspaceImageResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-import-workspace-image-result-schema.json\",\n  \"description\": \"ImportWorkspaceImageResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-import-workspace-image-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ImportWorkspaceImageResult
---
