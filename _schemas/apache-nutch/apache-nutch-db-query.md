---
description: Parameters for a CrawlDB query.
layout: schema
name: DbQuery
properties_list:
- description: Configuration ID. Falls back to "default" if not provided.
  name: confId
  type: string
- description: The type of CrawlDB query to execute.
  name: type
  type: string
- description: Additional arguments for the query.
  name: args
  type: object
- description: The crawl identifier.
  name: crawlId
  type: string
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-db-query-schema.json
slug: apache-nutch-db-query
source_filename: apache-nutch-db-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-db-query-schema.json\",\n  \"title\": \"DbQuery\",\n  \"description\": \"Parameters for a CrawlDB query.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"confId\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration ID. Falls back to \\\"default\\\" if not provided.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of CrawlDB query to execute.\",\n      \"enum\": [\n        \"stats\",\n        \"dump\",\n        \"topN\",\n        \"url\"\n      ]\n    },\n    \"args\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional arguments for the query.\"\n    },\n    \"crawlId\": {\n      \"type\": \"string\",\n      \"description\": \"The crawl\
  \ identifier.\"\n    }\n  },\n  \"required\": [\n    \"crawlId\",\n    \"type\"\n  ],\n  \"example\": {\n    \"confId\": \"default\",\n    \"type\": \"stats\",\n    \"crawlId\": \"crawl-01\",\n    \"args\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-db-query-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: DbQuery
---
