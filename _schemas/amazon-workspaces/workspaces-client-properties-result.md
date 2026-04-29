---
description: Information about the Amazon WorkSpaces client.
layout: schema
name: ClientPropertiesResult
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: ClientProperties
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-client-properties-result-schema.json
slug: workspaces-client-properties-result
source_filename: workspaces-client-properties-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The resource identifier, in the form of a directory ID.\"\n        }\n      ]\n    },\n    \"ClientProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientProperties\"\n        },\n        {\n          \"description\": \"Information about the Amazon WorkSpaces client.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Information about the Amazon WorkSpaces client.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClientPropertiesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-client-properties-result-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-client-properties-result-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ClientPropertiesResult
---
