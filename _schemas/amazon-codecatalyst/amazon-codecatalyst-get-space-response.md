---
description: GetSpaceResponse schema from Amazon CodeCatalyst
layout: schema
name: GetSpaceResponse
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: regionName
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-get-space-response-schema.json
slug: amazon-codecatalyst-get-space-response
source_filename: amazon-codecatalyst-get-space-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-get-space-response-schema.json\",\n  \"title\": \"GetSpaceResponse\",\n  \"description\": \"GetSpaceResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the space.\"\n        }\n      ]\n    },\n    \"regionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegionString\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region where the space exists.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n    \
  \      \"description\": \"The friendly name of the space displayed to users.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The description of the space.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"regionName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-get-space-response-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: GetSpaceResponse
---
