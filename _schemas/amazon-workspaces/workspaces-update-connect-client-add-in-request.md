---
description: UpdateConnectClientAddInRequest schema from Amazon WorkSpaces API
layout: schema
name: UpdateConnectClientAddInRequest
properties_list:
- description: ''
  name: AddInId
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: URL
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-update-connect-client-add-in-request-schema.json
slug: workspaces-update-connect-client-add-in-request
source_filename: workspaces-update-connect-client-add-in-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"AddInId\",\n    \"ResourceId\"\n  ],\n  \"title\": \"UpdateConnectClientAddInRequest\",\n  \"properties\": {\n    \"AddInId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonUuid\"\n        },\n        {\n          \"description\": \"The identifier of the client add-in to update.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The directory identifier for which the client add-in is configured.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddInName\"\n        },\n        {\n          \"description\": \"The name of the client add-in.\"\n        }\n      ]\n    },\n    \"URL\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddInUrl\"\n   \
  \     },\n        {\n          \"description\": \"The endpoint URL of the Amazon Connect client add-in.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-update-connect-client-add-in-request-schema.json\",\n  \"description\": \"UpdateConnectClientAddInRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-update-connect-client-add-in-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: UpdateConnectClientAddInRequest
---
