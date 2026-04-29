---
description: DeleteWorkspaceBundleRequest schema from Amazon WorkSpaces API
layout: schema
name: DeleteWorkspaceBundleRequest
properties_list:
- description: ''
  name: BundleId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-delete-workspace-bundle-request-schema.json
slug: workspaces-delete-workspace-bundle-request
source_filename: workspaces-delete-workspace-bundle-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"DeleteWorkspaceBundleRequest\",\n  \"properties\": {\n    \"BundleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BundleId\"\n        },\n        {\n          \"description\": \"The identifier of the bundle.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-delete-workspace-bundle-request-schema.json\",\n  \"description\": \"DeleteWorkspaceBundleRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-delete-workspace-bundle-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DeleteWorkspaceBundleRequest
---
