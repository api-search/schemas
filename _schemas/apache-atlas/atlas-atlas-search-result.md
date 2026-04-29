---
description: Result of a search query against the Atlas metadata repository.
layout: schema
name: AtlasSearchResult
properties_list:
- description: Type of search query executed.
  name: queryType
  type: string
- description: The search parameters that were used.
  name: searchParameters
  type: object
- description: List of matching entity headers.
  name: entities
  type: array
- description: Approximate total count of matching entities.
  name: approximateCount
  type: integer
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-atlas-search-result-schema.json
slug: atlas-atlas-search-result
source_filename: atlas-atlas-search-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-search-result-schema.json\",\n  \"title\": \"AtlasSearchResult\",\n  \"description\": \"Result of a search query against the Atlas metadata repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queryType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of search query executed.\",\n      \"example\": \"BASIC\"\n    },\n    \"searchParameters\": {\n      \"type\": \"object\",\n      \"description\": \"The search parameters that were used.\"\n    },\n    \"entities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"List of matching entity headers.\"\n    },\n    \"approximateCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Approximate total count of matching entities.\",\n      \"\
  example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-search-result-schema.json
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: AtlasSearchResult
---
