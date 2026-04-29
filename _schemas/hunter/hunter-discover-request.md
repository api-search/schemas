---
description: ''
layout: schema
name: DiscoverRequest
properties_list:
- description: Natural language search query to find matching companies.
  name: query
  type: string
- description: Filter by organization attributes.
  name: organization
  type: object
- description: Filter by geographic location of headquarters.
  name: headquarters_location
  type: object
- description: Filter by industry classification.
  name: industry
  type: object
- description: Filter by company headcount ranges.
  name: headcount
  type: array
- description: Filter by company entity type.
  name: company_type
  type: object
- description: Filter by year the company was founded.
  name: year_founded
  type: object
- description: Filter by technologies used by the company.
  name: technology
  type: object
- description: Filter by business keywords.
  name: keywords
  type: object
- description: Filter by funding information.
  name: funding
  type: object
- description: Maximum number of results to return.
  name: limit
  type: integer
- description: Number of results to skip for pagination.
  name: offset
  type: integer
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-discover-request-schema.json
slug: hunter-discover-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DiscoverRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"Natural language search query to find matching companies.\"\n    },\n    \"organization\": {\n      \"type\": \"object\",\n      \"description\": \"Filter by organization attributes.\"\n    },\n    \"headquarters_location\": {\n      \"type\": \"object\",\n      \"description\": \"Filter by geographic location of headquarters.\"\n    },\n    \"industry\": {\n      \"type\": \"object\",\n      \"description\": \"Filter by industry classification.\"\n    },\n    \"headcount\": {\n      \"type\": \"array\",\n      \"description\": \"Filter by company headcount ranges.\"\n    },\n    \"company_type\": {\n      \"type\": \"object\",\n      \"description\": \"Filter by company entity type.\"\n    },\n    \"year_founded\": {\n      \"type\": \"object\",\n      \"\
  description\": \"Filter by year the company was founded.\"\n    },\n    \"technology\": {\n      \"type\": \"object\",\n      \"description\": \"Filter by technologies used by the company.\"\n    },\n    \"keywords\": {\n      \"type\": \"object\",\n      \"description\": \"Filter by business keywords.\"\n    },\n    \"funding\": {\n      \"type\": \"object\",\n      \"description\": \"Filter by funding information.\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of results to return.\"\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of results to skip for pagination.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-discover-request-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: DiscoverRequest
---
