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
schema_file: json-schema/log-api-common-block-schema.json
slug: log-api-common-block
source_filename: log-api-common-block-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/log-api-common-block-schema.json\",\n  \"title\": \"CommonBlock\",\n  \"description\": \"Shared attributes applied to all log records in this batch\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Default Unix timestamp in milliseconds for all logs in the batch\",\n      \"example\": 1718153645993\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value attributes applied to all logs in this batch\",\n      \"additionalProperties\": {\n        \"oneOf\": [\n          {\n            \"type\": \"string\"\n          },\n          {\n            \"type\": \"number\"\n          },\n          {\n            \"type\": \"boolean\"\n          }\n        ]\n      },\n      \"example\": {\n        \"customAttribute\"\
  : \"example_value\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/log-api-common-block-schema.json
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
