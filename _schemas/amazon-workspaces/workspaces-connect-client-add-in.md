---
description: Describes an Amazon Connect client add-in.
layout: schema
name: ConnectClientAddIn
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
schema_file: json-schema/workspaces-connect-client-add-in-schema.json
slug: workspaces-connect-client-add-in
source_filename: workspaces-connect-client-add-in-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AddInId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonUuid\"\n        },\n        {\n          \"description\": \"The client add-in identifier.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The directory identifier for which the client add-in is configured.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddInName\"\n        },\n        {\n          \"description\": \"The name of the client add in.\"\n        }\n      ]\n    },\n    \"URL\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddInUrl\"\n        },\n        {\n          \"description\": \"The endpoint URL of the client add-in.\"\n        }\n      ]\n    }\n  },\n  \"description\"\
  : \"Describes an Amazon Connect client add-in.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConnectClientAddIn\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-connect-client-add-in-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-connect-client-add-in-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ConnectClientAddIn
---
