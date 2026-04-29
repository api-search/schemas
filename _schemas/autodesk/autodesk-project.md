---
description: A project represents a design or construction project within a hub. Projects contain folders, items, and versions that organize the project's design data and documents.
layout: schema
name: Autodesk Project
properties_list:
- description: The JSON:API resource type.
  name: type
  type: string
- description: The unique project identifier, prefixed with 'b.' for BIM 360/ACC projects.
  name: id
  type: string
- description: ''
  name: attributes
  type: object
- description: ''
  name: relationships
  type: object
provider_name: Autodesk
provider_slug: autodesk
schema_file: json-schema/autodesk-project.json
slug: autodesk-project
source_filename: autodesk-project.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-search/autodesk/refs/heads/main/json-schema/autodesk-project.json\",\n  \"title\": \"Autodesk Project\",\n  \"description\": \"A project represents a design or construction project within a hub. Projects contain folders, items, and versions that organize the project's design data and documents.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"projects\",\n      \"description\": \"The JSON:API resource type.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique project identifier, prefixed with 'b.' for BIM 360/ACC projects.\",\n      \"examples\": [\"b.12345678-abcd-efgh-ijkl-123456789012\"]\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The display name of the project.\"\n        },\n        \"scopes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Access scopes the user has on this project.\"\n        },\n        \"extension\": {\n          \"$ref\": \"#/$defs/Extension\"\n        }\n      },\n      \"required\": [\"name\"]\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"hub\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"data\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"const\": \"hubs\"\n                },\n                \"id\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        },\n        \"rootFolder\": {\n          \"type\": \"object\",\n          \"properties\"\
  : {\n            \"data\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"const\": \"folders\"\n                },\n                \"id\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        },\n        \"topFolders\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"links\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"related\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"href\": {\n                      \"type\": \"string\",\n                      \"format\": \"uri\"\n                    }\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"issues\": {\n          \"type\": \"object\",\n          \"properties\": {\n   \
  \         \"data\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\"\n                },\n                \"id\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"type\", \"id\"],\n  \"$defs\": {\n    \"Extension\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"examples\": [\"projects:autodesk.bim360:Project\", \"projects:autodesk.core:Project\"]\n        },\n        \"version\": {\n          \"type\": \"string\"\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/json-schema/autodesk-project.json
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
title: Autodesk Project
---
