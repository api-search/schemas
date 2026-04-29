---
description: An analytics segment definition
layout: schema
name: Segment
properties_list:
- description: Unique segment identifier
  name: id
  type: string
- description: Display name of the segment
  name: name
  type: string
- description: Description of the segment's purpose
  name: description
  type: string
- description: The report suite this segment is based on
  name: rsid
  type: string
- description: The owner of an Analytics component
  name: owner
  type: object
- description: The segment rule definition
  name: definition
  type: object
- description: Last modification timestamp
  name: modified
  type: string
- description: ''
  name: tags
  type: array
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-segment-schema.json
slug: adobe-analytics-segment
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"An analytics segment definition\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique segment identifier\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the segment\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the segment's purpose\",\n      \"example\": \"A sample description.\"\n    },\n    \"rsid\": {\n      \"type\": \"string\",\n      \"description\": \"The report suite this segment is based on\",\n      \"example\": \"500123\"\n    },\n    \"owner\": {\n      \"type\": \"object\",\n      \"description\": \"The owner of an Analytics component\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Owner user ID\",\n          \"example\": \"abc123\"\
  \n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Owner display name\",\n          \"example\": \"Example Title\"\n        },\n        \"login\": {\n          \"type\": \"string\",\n          \"description\": \"Owner login identifier\",\n          \"example\": \"example_value\"\n        }\n      }\n    },\n    \"definition\": {\n      \"type\": \"object\",\n      \"description\": \"The segment rule definition\",\n      \"example\": \"example_value\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"description\": \"Last modification timestamp\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A tag applied to an Analytics component\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\"\
  : \"Tag identifier\",\n            \"example\": \"abc123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Tag name\",\n            \"example\": \"Example Title\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Tag description\",\n            \"example\": \"A sample description.\"\n          },\n          \"components\": {\n            \"type\": \"array\",\n            \"description\": \"List of components this tag is applied to\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Segment\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-segment-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: Segment
---
