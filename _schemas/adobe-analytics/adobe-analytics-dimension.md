---
description: An analytics dimension available in a report suite
layout: schema
name: Dimension
properties_list:
- description: Dimension ID (e.g. variables/page)
  name: id
  type: string
- description: Display name of the dimension
  name: title
  type: string
- description: Internal name
  name: name
  type: string
- description: Dimension data type
  name: type
  type: string
- description: Category grouping for the dimension
  name: category
  type: string
- description: Description of what the dimension tracks
  name: description
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-dimension-schema.json
slug: adobe-analytics-dimension
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"An analytics dimension available in a report suite\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Dimension ID (e.g. variables/page)\",\n      \"example\": \"abc123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the dimension\",\n      \"example\": \"Example Title\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Internal name\",\n      \"example\": \"Example Title\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Dimension data type\",\n      \"example\": \"example_value\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category grouping for the dimension\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what the dimension tracks\",\n   \
  \   \"example\": \"A sample description.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Dimension\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-dimension-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: Dimension
---
