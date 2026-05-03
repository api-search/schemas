---
description: A Zesty.io media file represents an uploaded asset (image, document, video, etc.) stored in a media bin and served via CDN.
layout: schema
name: Zesty Media File
properties_list:
- description: The Zesty Universal Identifier for the file.
  name: ZUID
  type: string
- description: The bin ZUID this file belongs to.
  name: binZUID
  type: string
- description: The group ZUID this file belongs to.
  name: groupZUID
  type: string
- description: The file name.
  name: fileName
  type: string
- description: The display title of the file.
  name: title
  type: string
- description: The CDN URL for the file.
  name: url
  type: string
- description: The MIME type of the file.
  name: type
  type: string
- description: Timestamp when the file was uploaded.
  name: createdAt
  type: string
- description: Timestamp when the file was last updated.
  name: updatedAt
  type: string
provider_name: Zesty
provider_slug: zesty
schema_file: json-schema/media-file.json
slug: media-file
source_filename: media-file.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zesty/blob/main/json-schema/media-file.json\",\n  \"title\": \"Zesty Media File\",\n  \"description\": \"A Zesty.io media file represents an uploaded asset (image, document, video, etc.) stored in a media bin and served via CDN.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The Zesty Universal Identifier for the file.\"\n    },\n    \"binZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The bin ZUID this file belongs to.\"\n    },\n    \"groupZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The group ZUID this file belongs to.\"\n    },\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"The file name.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The display title of the file.\"\n    },\n    \"\
  url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The CDN URL for the file.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The MIME type of the file.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the file was uploaded.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the file was last updated.\"\n    }\n  },\n  \"required\": [\"ZUID\", \"binZUID\", \"fileName\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/json-schema/media-file.json
tags:
- CMS
- Composable
- Content Management
- Headless CMS
- Media
title: Zesty Media File
---
