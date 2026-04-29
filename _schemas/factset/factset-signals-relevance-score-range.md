---
description: 'Represents a valid range for user relevancy score for signal events. The upper bound of the range is represented by the attribute **gt** or **gte**. The lower bound of the range is presented by **lt** or **lte** The range can contain either of the bounds or both. e.g. { "gt": 0.4, "lt": 0.8 }'
layout: schema
name: RelevanceScoreRange
properties_list:
- description: ''
  name: gt
  type: number
- description: ''
  name: gte
  type: number
- description: ''
  name: lt
  type: number
- description: ''
  name: lte
  type: number
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-signals-relevance-score-range-schema.json
slug: factset-signals-relevance-score-range
source_filename: factset-signals-relevance-score-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RelevanceScoreRange\",\n  \"type\": \"object\",\n  \"description\": \"Represents a valid range for user relevancy score for signal events. The upper bound of the range is represented by the attribute **gt** or **gte**. The lower bound of the range is presented by **lt** or **lte** The range can contain either of the bounds or both. e.g. { \\\"gt\\\": 0.4, \\\"lt\\\": 0.8 }\\n\",\n  \"properties\": {\n    \"gt\": {\n      \"type\": \"number\"\n    },\n    \"gte\": {\n      \"type\": \"number\"\n    },\n    \"lt\": {\n      \"type\": \"number\"\n    },\n    \"lte\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-signals-relevance-score-range-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: RelevanceScoreRange
---
