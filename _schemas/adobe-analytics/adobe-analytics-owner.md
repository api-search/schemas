---
description: The owner of an Analytics component
layout: schema
name: Owner
properties_list:
- description: Owner user ID
  name: id
  type: integer
- description: Owner display name
  name: name
  type: string
- description: Owner login identifier
  name: login
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-owner-schema.json
slug: adobe-analytics-owner
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The owner of an Analytics component\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Owner user ID\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Owner display name\",\n      \"example\": \"Example Title\"\n    },\n    \"login\": {\n      \"type\": \"string\",\n      \"description\": \"Owner login identifier\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Owner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-owner-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: Owner
---
