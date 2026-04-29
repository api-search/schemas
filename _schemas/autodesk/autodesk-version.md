---
description: A version represents a specific revision of an item in the Autodesk Data Management system. Each time a file is uploaded or modified, a new version is created, enabling version history tracking and rollback capabilities.
layout: schema
name: Autodesk Version
properties_list:
- description: The JSON:API resource type.
  name: type
  type: string
- description: The unique version identifier (URN).
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
schema_file: json-schema/autodesk-version.json
slug: autodesk-version
source_filename: autodesk-version.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-search/autodesk/refs/heads/main/json-schema/autodesk-version.json\",\n  \"title\": \"Autodesk Version\",\n  \"description\": \"A version represents a specific revision of an item in the Autodesk Data Management system. Each time a file is uploaded or modified, a new version is created, enabling version history tracking and rollback capabilities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"versions\",\n      \"description\": \"The JSON:API resource type.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique version identifier (URN).\",\n      \"examples\": [\"urn:adsk.wipprod:fs.file:vf.abcdefgh-1234?version=1\"]\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"The version name/filename.\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name.\"\n        },\n        \"versionNumber\": {\n          \"type\": \"integer\",\n          \"description\": \"The version number (1-based).\",\n          \"minimum\": 1\n        },\n        \"mimeType\": {\n          \"type\": \"string\",\n          \"description\": \"The MIME type of the file.\"\n        },\n        \"fileType\": {\n          \"type\": \"string\",\n          \"description\": \"The file extension.\"\n        },\n        \"storageSize\": {\n          \"type\": \"integer\",\n          \"description\": \"The file size in bytes.\"\n        },\n        \"createTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"createUserId\": {\n          \"type\": \"string\"\n        },\n        \"createUserName\": {\n          \"type\": \"string\"\n        },\n \
  \       \"lastModifiedTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"lastModifiedUserId\": {\n          \"type\": \"string\"\n        },\n        \"lastModifiedUserName\": {\n          \"type\": \"string\"\n        },\n        \"extension\": {\n          \"$ref\": \"#/$defs/Extension\"\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"item\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"data\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"const\": \"items\"\n                },\n                \"id\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        },\n        \"storage\": {\n          \"type\": \"object\",\n          \"properties\": {\n          \
  \  \"data\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"const\": \"objects\"\n                },\n                \"id\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        },\n        \"derivatives\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"data\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\"\n                },\n                \"id\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"type\", \"id\"],\n  \"$defs\": {\n    \"Extension\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"examples\"\
  : [\n            \"versions:autodesk.bim360:File\",\n            \"versions:autodesk.core:File\",\n            \"versions:autodesk.bim360:C4RModel\"\n          ]\n        },\n        \"version\": {\n          \"type\": \"string\"\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/json-schema/autodesk-version.json
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
title: Autodesk Version
---
