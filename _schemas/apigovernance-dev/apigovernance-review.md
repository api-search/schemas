---
description: An automated API governance review result.
layout: schema
name: Review
properties_list:
- description: Review identifier.
  name: id
  type: string
- description: URL of the reviewed API specification.
  name: apiSpecUrl
  type: string
- description: Overall governance score.
  name: score
  type: number
- description: Number of guideline violations found.
  name: violations
  type: integer
- description: When the review was created.
  name: createdAt
  type: string
- description: Review status.
  name: status
  type: string
provider_name: APIGovernance.Dev
provider_slug: apigovernance-dev
schema_file: json-schema/apigovernance-review-schema.json
slug: apigovernance-review
source_filename: apigovernance-review-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apigovernance-dev/refs/heads/main/json-schema/apigovernance-review-schema.json\",\n  \"title\": \"Review\",\n  \"description\": \"An automated API governance review result.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Review identifier.\",\n      \"example\": \"rev-001\"\n    },\n    \"apiSpecUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the reviewed API specification.\"\n    },\n    \"score\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Overall governance score.\",\n      \"example\": 87.5\n    },\n    \"violations\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of guideline violations found.\",\n      \"example\": 3\n    },\n    \"createdAt\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the review was created.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"passed\",\n        \"failed\",\n        \"warning\"\n      ],\n      \"description\": \"Review status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigovernance-dev/refs/heads/main/json-schema/apigovernance-review-schema.json
tags:
- API Design
- API Governance
- Best Practices
- Compliance
- Guidelines
- Standards
title: Review
---
