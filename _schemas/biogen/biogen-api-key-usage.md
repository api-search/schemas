---
description: Usage statistics for an API key.
layout: schema
name: ApiKeyUsage
properties_list:
- description: Number of requests made today.
  name: requests_today
  type: integer
- description: Number of requests made this month.
  name: requests_month
  type: integer
provider_name: Biogen
provider_slug: biogen
schema_file: json-schema/biogen-api-key-usage-schema.json
slug: biogen-api-key-usage
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ApiKeyUsage\",\n  \"type\": \"object\",\n  \"description\": \"Usage statistics for an API key.\",\n  \"properties\": {\n    \"requests_today\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of requests made today.\",\n      \"example\": 150\n    },\n    \"requests_month\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of requests made this month.\",\n      \"example\": 4200\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/json-schema/biogen-api-key-usage-schema.json
tags:
- Biotechnology
- Healthcare
- Life Sciences
- Pharmaceuticals
- Neurology
title: ApiKeyUsage
---
