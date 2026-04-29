---
description: Shared attributes applied to all metrics in this data object unless overridden at the metric level
layout: schema
name: CommonBlock
properties_list:
- description: Unix timestamp in milliseconds for all metrics in this batch
  name: timestamp
  type: integer
- description: Default measurement interval in milliseconds for count and summary metrics
  name: interval.ms
  type: integer
- description: Key-value pairs applied to all metrics in the batch. Values can be strings, numbers, or booleans.
  name: attributes
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/metric-api-common-block-schema.json
slug: metric-api-common-block
source_filename: metric-api-common-block-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/metric-api-common-block-schema.json\",\n  \"title\": \"CommonBlock\",\n  \"description\": \"Shared attributes applied to all metrics in this data object unless overridden at the metric level\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in milliseconds for all metrics in this batch\",\n      \"example\": 1718153645993\n    },\n    \"interval.ms\": {\n      \"type\": \"integer\",\n      \"description\": \"Default measurement interval in milliseconds for count and summary metrics\",\n      \"example\": 100\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs applied to all metrics in the batch. Values can be strings, numbers, or booleans.\",\n      \"additionalProperties\"\
  : {\n        \"oneOf\": [\n          {\n            \"type\": \"string\"\n          },\n          {\n            \"type\": \"number\"\n          },\n          {\n            \"type\": \"boolean\"\n          }\n        ]\n      },\n      \"example\": {\n        \"customAttribute\": \"example_value\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/metric-api-common-block-schema.json
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
title: CommonBlock
---
