---
description: UpdateWorkspaceImagePermissionRequest schema from Amazon WorkSpaces API
layout: schema
name: UpdateWorkspaceImagePermissionRequest
properties_list:
- description: ''
  name: ImageId
  type: object
- description: ''
  name: AllowCopyImage
  type: object
- description: ''
  name: SharedAccountId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-update-workspace-image-permission-request-schema.json
slug: workspaces-update-workspace-image-permission-request
source_filename: workspaces-update-workspace-image-permission-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ImageId\",\n    \"AllowCopyImage\",\n    \"SharedAccountId\"\n  ],\n  \"title\": \"UpdateWorkspaceImagePermissionRequest\",\n  \"properties\": {\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageId\"\n        },\n        {\n          \"description\": \"The identifier of the image.\"\n        }\n      ]\n    },\n    \"AllowCopyImage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"The permission to copy the image. This permission can be revoked only after an image has been shared.\"\n        }\n      ]\n    },\n    \"SharedAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsAccount\"\n        },\n        {\n          \"description\": \"<p>The identifier of the Amazon Web Services account to share or unshare the image with.</p>\
  \ <important> <p>Before sharing the image, confirm that you are sharing to the correct Amazon Web Services account ID.</p> </important>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-update-workspace-image-permission-request-schema.json\",\n  \"description\": \"UpdateWorkspaceImagePermissionRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-update-workspace-image-permission-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: UpdateWorkspaceImagePermissionRequest
---
