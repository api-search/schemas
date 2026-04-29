---
description: Metrics set representation.
layout: schema
name: MetricSet
properties_list:
- description: Metric set name.
  name: name
  type: string
- description: Metrics.
  name: metrics
  type: array
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-metric-set-schema.json
slug: rest-api-metric-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-metric-set-schema.json\",\n  \"title\": \"MetricSet\",\n  \"description\": \"Metrics set representation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Metric set name.\"\n    },\n    \"metrics\": {\n      \"type\": \"array\",\n      \"description\": \"Metrics.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Metric\"\n      }\n    }\n  },\n  \"required\": [\n    \"metrics\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-metric-set-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: MetricSet
---
