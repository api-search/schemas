---
description: A content item in the Seismic platform representing a document, presentation, or other sales enablement material.
layout: schema
name: Seismic Content Item
properties_list:
- description: Unique identifier of the content item.
  name: id
  type: string
- description: Name of the content item.
  name: name
  type: string
- description: Description of the content item.
  name: description
  type: string
- description: ID of the folder containing this content item.
  name: folderId
  type: string
- description: ID of the associated content profile.
  name: contentProfileId
  type: string
- description: File type extension of the content item.
  name: fileType
  type: string
- description: File size in bytes.
  name: fileSize
  type: integer
- description: MIME type of the content file.
  name: mimeType
  type: string
- description: Current version number of the content item.
  name: versionNumber
  type: integer
- description: Publication status of the content item.
  name: status
  type: string
- description: Tags associated with the content item.
  name: tags
  type: array
- description: Custom content property values as key-value pairs.
  name: properties
  type: object
- description: ID of the user who created the content item.
  name: createdBy
  type: string
- description: Timestamp when the content item was created.
  name: createdAt
  type: string
- description: ID of the user who last modified the content item.
  name: modifiedBy
  type: string
- description: Timestamp when the content item was last modified.
  name: modifiedAt
  type: string
- description: URL for the content item thumbnail image.
  name: thumbnailUrl
  type: string
provider_name: Seismic
provider_slug: seismic
schema_file: json-schema/seismic-content-item-schema.json
slug: seismic-content-item
source_filename: seismic-content-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.seismic.com/schemas/content-item\",\n  \"title\": \"Seismic Content Item\",\n  \"description\": \"A content item in the Seismic platform representing a document, presentation, or other sales enablement material.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the content item.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the content item.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the content item.\"\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the folder containing this content item.\"\n    },\n    \"contentProfileId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the associated content profile.\"\n    },\n    \"fileType\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"File type extension of the content item.\",\n      \"examples\": [\"pdf\", \"pptx\", \"docx\", \"xlsx\", \"png\", \"mp4\"]\n    },\n    \"fileSize\": {\n      \"type\": \"integer\",\n      \"description\": \"File size in bytes.\",\n      \"minimum\": 0\n    },\n    \"mimeType\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the content file.\",\n      \"examples\": [\"application/pdf\", \"application/vnd.openxmlformats-officedocument.presentationml.presentation\"]\n    },\n    \"versionNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Current version number of the content item.\",\n      \"minimum\": 1\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Publication status of the content item.\",\n      \"enum\": [\"draft\", \"published\", \"archived\"]\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n \
  \     },\n      \"description\": \"Tags associated with the content item.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Custom content property values as key-value pairs.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who created the content item.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the content item was created.\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who last modified the content item.\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the content item was last modified.\"\n    },\n    \"thumbnailUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"\
  description\": \"URL for the content item thumbnail image.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/json-schema/seismic-content-item-schema.json
tags: []
title: Seismic Content Item
---
