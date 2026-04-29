---
description: UpdateWorkspaceBundleRequest schema from Amazon WorkSpaces API
layout: schema
name: UpdateWorkspaceBundleRequest
properties_list:
- description: ''
  name: BundleId
  type: object
- description: ''
  name: ImageId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-update-workspace-bundle-request-schema.json
slug: workspaces-update-workspace-bundle-request
source_filename: workspaces-update-workspace-bundle-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"UpdateWorkspaceBundleRequest\",\n  \"properties\": {\n    \"BundleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BundleId\"\n        },\n        {\n          \"description\": \"The identifier of the bundle.\"\n        }\n      ]\n    },\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageId\"\n        },\n        {\n          \"description\": \"The identifier of the image.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-update-workspace-bundle-request-schema.json\",\n  \"description\": \"UpdateWorkspaceBundleRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-update-workspace-bundle-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: UpdateWorkspaceBundleRequest
---
