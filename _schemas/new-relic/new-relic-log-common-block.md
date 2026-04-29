---
description: Shared attributes applied to all log records in this batch
layout: schema
name: CommonBlock
properties_list:
- description: Default Unix timestamp in milliseconds for all logs in the batch
  name: timestamp
  type: integer
- description: Key-value attributes applied to all logs in this batch
  name: attributes
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-log-common-block-schema.json
slug: new-relic-log-common-block
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Shared attributes applied to all log records in this batch\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Default Unix timestamp in milliseconds for all logs in the batch\",\n      \"example\": 1718153645993\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value attributes applied to all logs in this batch\",\n      \"example\": {\n        \"customAttribute\": \"example_value\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommonBlock\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-log-common-block-schema.json
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
