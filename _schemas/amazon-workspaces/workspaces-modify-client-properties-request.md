---
description: ModifyClientPropertiesRequest schema from Amazon WorkSpaces API
layout: schema
name: ModifyClientPropertiesRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: ClientProperties
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-modify-client-properties-request-schema.json
slug: workspaces-modify-client-properties-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceId\",\n    \"ClientProperties\"\n  ],\n  \"title\": \"ModifyClientPropertiesRequest\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The resource identifiers, in the form of directory IDs.\"\n        }\n      ]\n    },\n    \"ClientProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientProperties\"\n        },\n        {\n          \"description\": \"Information about the Amazon WorkSpaces client.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-client-properties-request-schema.json\",\n  \"description\": \"ModifyClientPropertiesRequest schema from Amazon WorkSpaces\
  \ API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-client-properties-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ModifyClientPropertiesRequest
---
