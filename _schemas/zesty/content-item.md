---
description: A Zesty.io content item is an individual piece of content belonging to a content model. Items hold field data and have versioning and publishing states.
layout: schema
name: Zesty Content Item
properties_list:
- description: The Zesty Universal Identifier for the content item.
  name: ZUID
  type: string
- description: The content model ZUID this item belongs to.
  name: modelZUID
  type: string
- description: The field data for the content item.
  name: data
  type: object
- description: Web-specific metadata for the content item.
  name: web
  type: object
- description: Metadata about the content item.
  name: meta
  type: object
- description: Publishing state information.
  name: publishing
  type: object
provider_name: Zesty
provider_slug: zesty
schema_file: json-schema/content-item.json
slug: content-item
source_filename: content-item.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zesty/blob/main/json-schema/content-item.json\",\n  \"title\": \"Zesty Content Item\",\n  \"description\": \"A Zesty.io content item is an individual piece of content belonging to a content model. Items hold field data and have versioning and publishing states.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The Zesty Universal Identifier for the content item.\"\n    },\n    \"modelZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The content model ZUID this item belongs to.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The field data for the content item.\",\n      \"additionalProperties\": true\n    },\n    \"web\": {\n      \"type\": \"object\",\n      \"description\": \"Web-specific metadata for the content item.\",\n      \"properties\"\
  : {\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"The URL path for the content item.\"\n        },\n        \"pathPart\": {\n          \"type\": \"string\",\n          \"description\": \"The URL path part for this item.\"\n        },\n        \"metaTitle\": {\n          \"type\": \"string\",\n          \"description\": \"The meta title for SEO.\"\n        },\n        \"metaDescription\": {\n          \"type\": \"string\",\n          \"description\": \"The meta description for SEO.\"\n        },\n        \"canonicalTagMode\": {\n          \"type\": \"integer\",\n          \"description\": \"The canonical tag mode.\"\n        }\n      }\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about the content item.\",\n      \"properties\": {\n        \"version\": {\n          \"type\": \"integer\",\n          \"description\": \"The current version number.\"\n        },\n        \"listed\": {\n          \"type\": \"boolean\"\
  ,\n          \"description\": \"Whether the item is listed in navigation.\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the item was created.\"\n        },\n        \"updatedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the item was last updated.\"\n        }\n      }\n    },\n    \"publishing\": {\n      \"type\": \"object\",\n      \"description\": \"Publishing state information.\",\n      \"properties\": {\n        \"isPublished\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the item is currently published.\"\n        },\n        \"publishAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Scheduled publish date.\"\n        },\n        \"unpublishAt\": {\n          \"type\": \"string\",\n          \"format\": \"\
  date-time\",\n          \"description\": \"Scheduled unpublish date.\"\n        }\n      }\n    }\n  },\n  \"required\": [\"ZUID\", \"modelZUID\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/json-schema/content-item.json
tags:
- CMS
- Composable
- Content Management
- Headless CMS
- Media
title: Zesty Content Item
---
