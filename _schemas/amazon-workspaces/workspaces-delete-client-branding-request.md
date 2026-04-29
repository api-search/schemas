---
description: DeleteClientBrandingRequest schema from Amazon WorkSpaces API
layout: schema
name: DeleteClientBrandingRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: Platforms
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-delete-client-branding-request-schema.json
slug: workspaces-delete-client-branding-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceId\",\n    \"Platforms\"\n  ],\n  \"title\": \"DeleteClientBrandingRequest\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The directory identifier of the WorkSpace for which you want to delete client branding.\"\n        }\n      ]\n    },\n    \"Platforms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientDeviceTypeList\"\n        },\n        {\n          \"description\": \"The device type for which you want to delete client branding.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-delete-client-branding-request-schema.json\",\n  \"description\": \"DeleteClientBrandingRequest\
  \ schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-delete-client-branding-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DeleteClientBrandingRequest
---
