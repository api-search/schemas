---
description: JSON:API resource representation of a DatoCMS record (item).
layout: schema
name: DatoCMS Item
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: id
  type: string
- description: Field values keyed by API key.
  name: attributes
  type: object
- description: ''
  name: relationships
  type: object
- description: ''
  name: meta
  type: object
provider_name: DatoCMS
provider_slug: datocms
schema_file: json-schema/item.json
slug: item
source_filename: item.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datocms/main/json-schema/item.json\",\n  \"title\": \"DatoCMS Item\",\n  \"description\": \"JSON:API resource representation of a DatoCMS record (item).\",\n  \"type\": \"object\",\n  \"required\": [\"type\", \"id\"],\n  \"properties\": {\n    \"type\": {\"type\": \"string\", \"const\": \"item\"},\n    \"id\": {\"type\": \"string\"},\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Field values keyed by API key.\",\n      \"additionalProperties\": true\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"item_type\": {\"type\": \"object\"},\n        \"creator\": {\"type\": \"object\"}\n      }\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"created_at\": {\"type\": \"string\", \"format\": \"date-time\"},\n        \"updated_at\": {\"\
  type\": \"string\", \"format\": \"date-time\"},\n        \"published_at\": {\"type\": \"string\", \"format\": \"date-time\"},\n        \"first_published_at\": {\"type\": \"string\", \"format\": \"date-time\"},\n        \"publication_scheduled_at\": {\"type\": [\"string\", \"null\"], \"format\": \"date-time\"},\n        \"unpublishing_scheduled_at\": {\"type\": [\"string\", \"null\"], \"format\": \"date-time\"},\n        \"status\": {\"type\": \"string\", \"enum\": [\"draft\", \"updated\", \"published\"]},\n        \"is_valid\": {\"type\": \"boolean\"}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datocms/refs/heads/main/json-schema/item.json
tags:
- CMS
- Content Delivery
- Content Management
- GraphQL
- Headless CMS
title: DatoCMS Item
---
