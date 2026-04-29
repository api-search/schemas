---
description: An item represents a file or document stored within a project folder in the Autodesk Data Management system. Items track version history and provide access to the underlying file data through version references.
layout: schema
name: Autodesk Item
properties_list:
- description: The JSON:API resource type.
  name: type
  type: string
- description: The unique item identifier (URN).
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
schema_file: json-schema/autodesk-item.json
slug: autodesk-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-search/autodesk/refs/heads/main/json-schema/autodesk-item.json\",\n  \"title\": \"Autodesk Item\",\n  \"description\": \"An item represents a file or document stored within a project folder in the Autodesk Data Management system. Items track version history and provide access to the underlying file data through version references.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"items\",\n      \"description\": \"The JSON:API resource type.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique item identifier (URN).\",\n      \"examples\": [\"urn:adsk.wipprod:dm.lineage:abcdefgh-1234\"]\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The display name of the item (typically the filename).\"\n        },\n        \"createTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the item was created.\"\n        },\n        \"createUserId\": {\n          \"type\": \"string\",\n          \"description\": \"The user ID who created the item.\"\n        },\n        \"createUserName\": {\n          \"type\": \"string\",\n          \"description\": \"The username who created the item.\"\n        },\n        \"lastModifiedTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the item was last modified.\"\n        },\n        \"lastModifiedUserId\": {\n          \"type\": \"string\"\n        },\n        \"lastModifiedUserName\": {\n          \"type\": \"string\"\n        },\n        \"hidden\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the item is hidden.\"\n        },\n   \
  \     \"reserved\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the item is reserved (checked out).\"\n        },\n        \"extension\": {\n          \"$ref\": \"#/$defs/Extension\"\n        }\n      },\n      \"required\": [\"displayName\"]\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"tip\": {\n          \"type\": \"object\",\n          \"description\": \"The latest version of this item.\",\n          \"properties\": {\n            \"data\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"const\": \"versions\"\n                },\n                \"id\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        },\n        \"versions\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"links\": {\n     \
  \         \"type\": \"object\",\n              \"properties\": {\n                \"related\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"href\": {\n                      \"type\": \"string\",\n                      \"format\": \"uri\"\n                    }\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"parent\": {\n          \"type\": \"object\",\n          \"description\": \"The parent folder.\",\n          \"properties\": {\n            \"data\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"const\": \"folders\"\n                },\n                \"id\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"type\", \"id\"],\n  \"$defs\": {\n \
  \   \"Extension\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"examples\": [\"items:autodesk.bim360:File\", \"items:autodesk.core:File\"]\n        },\n        \"version\": {\n          \"type\": \"string\"\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/json-schema/autodesk-item.json
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
title: Autodesk Item
---
