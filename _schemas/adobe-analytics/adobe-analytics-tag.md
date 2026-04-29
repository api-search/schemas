---
description: A tag applied to an Analytics component
layout: schema
name: Tag
properties_list:
- description: Tag identifier
  name: id
  type: integer
- description: Tag name
  name: name
  type: string
- description: Tag description
  name: description
  type: string
- description: List of components this tag is applied to
  name: components
  type: array
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-tag-schema.json
slug: adobe-analytics-tag
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A tag applied to an Analytics component\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Tag identifier\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Tag name\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Tag description\",\n      \"example\": \"A sample description.\"\n    },\n    \"components\": {\n      \"type\": \"array\",\n      \"description\": \"List of components this tag is applied to\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tag\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-tag-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: Tag
---
