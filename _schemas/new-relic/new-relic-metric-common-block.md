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
schema_file: json-schema/new-relic-metric-common-block-schema.json
slug: new-relic-metric-common-block
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Shared attributes applied to all metrics in this data object unless overridden at the metric level\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in milliseconds for all metrics in this batch\",\n      \"example\": 1718153645993\n    },\n    \"interval.ms\": {\n      \"type\": \"integer\",\n      \"description\": \"Default measurement interval in milliseconds for count and summary metrics\",\n      \"example\": 100\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs applied to all metrics in the batch. Values can be strings, numbers, or booleans.\",\n      \"example\": {\n        \"customAttribute\": \"example_value\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommonBlock\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-metric-common-block-schema.json
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
