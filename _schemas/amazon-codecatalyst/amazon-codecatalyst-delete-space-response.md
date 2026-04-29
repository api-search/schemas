---
description: DeleteSpaceResponse schema from Amazon CodeCatalyst
layout: schema
name: DeleteSpaceResponse
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: displayName
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-delete-space-response-schema.json
slug: amazon-codecatalyst-delete-space-response
source_filename: amazon-codecatalyst-delete-space-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-delete-space-response-schema.json\",\n  \"title\": \"DeleteSpaceResponse\",\n  \"description\": \"DeleteSpaceResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the space.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The friendly name of the space displayed to users of the space in Amazon CodeCatalyst.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-delete-space-response-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: DeleteSpaceResponse
---
