---
description: A Zesty.io media group is a folder within a media bin used to organize media files hierarchically.
layout: schema
name: Zesty Media Group
properties_list:
- description: The Zesty Universal Identifier for the group.
  name: ZUID
  type: string
- description: The name of the media group.
  name: name
  type: string
- description: The bin ZUID this group belongs to.
  name: binZUID
  type: string
- description: The parent group ZUID if nested.
  name: groupZUID
  type: string
- description: Timestamp when the group was created.
  name: createdAt
  type: string
- description: Timestamp when the group was last updated.
  name: updatedAt
  type: string
provider_name: Zesty
provider_slug: zesty
schema_file: json-schema/media-group.json
slug: media-group
source_filename: media-group.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zesty/blob/main/json-schema/media-group.json\",\n  \"title\": \"Zesty Media Group\",\n  \"description\": \"A Zesty.io media group is a folder within a media bin used to organize media files hierarchically.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The Zesty Universal Identifier for the group.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the media group.\"\n    },\n    \"binZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The bin ZUID this group belongs to.\"\n    },\n    \"groupZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The parent group ZUID if nested.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the group was\
  \ created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the group was last updated.\"\n    }\n  },\n  \"required\": [\"ZUID\", \"name\", \"binZUID\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/json-schema/media-group.json
tags:
- CMS
- Composable
- Content Management
- Headless CMS
- Media
title: Zesty Media Group
---
