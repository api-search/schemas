---
description: Metric representation.
layout: schema
name: Metric
properties_list:
- description: Metric name.
  name: name
  type: string
- description: Metric description.
  name: desc
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-metric-schema.json
slug: rest-api-metric
source_filename: rest-api-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-metric-schema.json\",\n  \"title\": \"Metric\",\n  \"description\": \"Metric representation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Metric name.\"\n    },\n    \"desc\": {\n      \"type\": \"string\",\n      \"description\": \"Metric description.\",\n      \"nullable\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-metric-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: Metric
---
