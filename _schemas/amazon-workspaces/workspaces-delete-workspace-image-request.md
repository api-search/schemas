---
description: DeleteWorkspaceImageRequest schema from Amazon WorkSpaces API
layout: schema
name: DeleteWorkspaceImageRequest
properties_list:
- description: ''
  name: ImageId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-delete-workspace-image-request-schema.json
slug: workspaces-delete-workspace-image-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ImageId\"\n  ],\n  \"title\": \"DeleteWorkspaceImageRequest\",\n  \"properties\": {\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageId\"\n        },\n        {\n          \"description\": \"The identifier of the image.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-delete-workspace-image-request-schema.json\",\n  \"description\": \"DeleteWorkspaceImageRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-delete-workspace-image-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DeleteWorkspaceImageRequest
---
