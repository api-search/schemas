---
description: A list of metric sources for a node.
layout: schema
name: NodeMetricSources
properties_list:
- description: Consistent id of the node.
  name: node
  type: string
- description: Metric sources.
  name: sources
  type: array
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-node-metric-sources-schema.json
slug: rest-api-node-metric-sources
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-node-metric-sources-schema.json\",\n  \"title\": \"NodeMetricSources\",\n  \"description\": \"A list of metric sources for a node.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"node\": {\n      \"type\": \"string\",\n      \"description\": \"Consistent id of the node.\"\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"description\": \"Metric sources.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MetricSource\"\n      }\n    }\n  },\n  \"required\": [\n    \"node\",\n    \"sources\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-node-metric-sources-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: NodeMetricSources
---
