---
description: A list of metric sources provided by modules.
layout: schema
name: MetricSource
properties_list:
- description: Metric source name.
  name: name
  type: string
- description: If True, the metric is tracked. Otherwise, the metric is not tracked.
  name: enabled
  type: boolean
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-metric-source-schema.json
slug: rest-api-metric-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-metric-source-schema.json\",\n  \"title\": \"MetricSource\",\n  \"description\": \"A list of metric sources provided by modules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Metric source name.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"If True, the metric is tracked. Otherwise, the metric is not tracked.\"\n    }\n  },\n  \"required\": [\n    \"enabled\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-metric-source-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: MetricSource
---
