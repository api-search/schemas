---
description: CreateConnectClientAddInRequest schema from Amazon WorkSpaces API
layout: schema
name: CreateConnectClientAddInRequest
properties_list:
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
schema_file: json-schema/workspaces-create-connect-client-add-in-request-schema.json
slug: workspaces-create-connect-client-add-in-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceId\",\n    \"Name\",\n    \"URL\"\n  ],\n  \"title\": \"CreateConnectClientAddInRequest\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The directory identifier for which to configure the client add-in.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddInName\"\n        },\n        {\n          \"description\": \"The name of the client add-in.\"\n        }\n      ]\n    },\n    \"URL\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddInUrl\"\n        },\n        {\n          \"description\": \"The endpoint URL of the Amazon Connect client add-in.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-connect-client-add-in-request-schema.json\"\
  ,\n  \"description\": \"CreateConnectClientAddInRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-connect-client-add-in-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateConnectClientAddInRequest
---
