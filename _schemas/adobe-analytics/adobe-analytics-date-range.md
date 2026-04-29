---
description: A saved date range component
layout: schema
name: DateRange
properties_list:
- description: Unique date range identifier
  name: id
  type: string
- description: Display name
  name: name
  type: string
- description: Description of the date range
  name: description
  type: string
- description: The date range definition expression
  name: definition
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-date-range-schema.json
slug: adobe-analytics-date-range
source_filename: adobe-analytics-date-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A saved date range component\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique date range identifier\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the date range\",\n      \"example\": \"A sample description.\"\n    },\n    \"definition\": {\n      \"type\": \"string\",\n      \"description\": \"The date range definition expression\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DateRange\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-date-range-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: DateRange
---
