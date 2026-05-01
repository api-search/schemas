---
description: Amazon Kendra query result containing ranked document passages and answers.
layout: schema
name: QueryResult
properties_list:
- description: The unique identifier for the query.
  name: QueryId
  type: string
- description: The results of the search query.
  name: ResultItems
  type: array
- description: The total number of items found.
  name: TotalNumberOfResults
  type: integer
- description: Contains the facet results.
  name: FacetResults
  type: array
provider_name: Amazon Kendra
provider_slug: amazon-kendra
schema_file: json-schema/amazon-kendra-query-result-schema.json
slug: amazon-kendra-query-result
source_filename: amazon-kendra-query-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/json-schema/amazon-kendra-query-result-schema.json\",\n  \"title\": \"QueryResult\",\n  \"description\": \"Amazon Kendra query result containing ranked document passages and answers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QueryId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the query.\",\n      \"example\": \"q-abc12345\"\n    },\n    \"ResultItems\": {\n      \"type\": \"array\",\n      \"description\": \"The results of the search query.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"TotalNumberOfResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of items found.\",\n      \"example\": 42\n    },\n    \"FacetResults\": {\n      \"type\": \"array\",\n      \"description\": \"Contains the facet results.\"\
  ,\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/json-schema/amazon-kendra-query-result-schema.json
tags:
- AI
- Enterprise Search
- Knowledge Management
- Machine Learning
- Natural Language
title: QueryResult
---
