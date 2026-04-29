---
description: A hub represents an Autodesk account (such as BIM 360, ACC, or Fusion Team) that serves as the top-level container for projects and data. Hubs provide organizational context for all data management operations.
layout: schema
name: Autodesk Hub
properties_list:
- description: The JSON:API resource type.
  name: type
  type: string
- description: The unique hub identifier, prefixed with 'b.' for BIM 360/ACC or 'a.' for Autodesk accounts.
  name: id
  type: string
- description: ''
  name: attributes
  type: object
- description: ''
  name: relationships
  type: object
- description: ''
  name: links
  type: object
provider_name: Autodesk
provider_slug: autodesk
schema_file: json-schema/autodesk-hub.json
slug: autodesk-hub
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-search/autodesk/refs/heads/main/json-schema/autodesk-hub.json\",\n  \"title\": \"Autodesk Hub\",\n  \"description\": \"A hub represents an Autodesk account (such as BIM 360, ACC, or Fusion Team) that serves as the top-level container for projects and data. Hubs provide organizational context for all data management operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"hubs\",\n      \"description\": \"The JSON:API resource type.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique hub identifier, prefixed with 'b.' for BIM 360/ACC or 'a.' for Autodesk accounts.\",\n      \"examples\": [\"b.12345678-abcd-efgh-ijkl-123456789012\"]\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"\
  type\": \"string\",\n          \"description\": \"The display name of the hub.\"\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"enum\": [\"US\", \"EMEA\"],\n          \"description\": \"The geographic region where the hub data is stored.\"\n        },\n        \"extension\": {\n          \"$ref\": \"#/$defs/Extension\"\n        }\n      },\n      \"required\": [\"name\"]\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"projects\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"links\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"related\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"href\": {\n                      \"type\": \"string\",\n                      \"format\": \"uri\"\n                    }\n                  }\n                }\n              }\n        \
  \    }\n          }\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"type\", \"id\"],\n  \"$defs\": {\n    \"Extension\": {\n      \"type\": \"object\",\n      \"description\": \"Extension object providing additional type-specific metadata.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The extension type identifier.\",\n          \"examples\": [\"hubs:autodesk.bim360:Account\", \"hubs:autodesk.core:Hub\"]\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"Extension schema version.\"\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"additionalProperties\"\
  : true\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/json-schema/autodesk-hub.json
tags:
- 3D Modeling
- Architecture
- BIM
- CAD
- Construction
- Design
- Digital Twins
- Engineering
- Manufacturing
- Media and Entertainment
- Sustainability
title: Autodesk Hub
---
