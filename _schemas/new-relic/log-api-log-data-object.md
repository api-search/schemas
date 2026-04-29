---
description: A batch of log records with optional shared attributes
layout: schema
name: LogDataObject
properties_list:
- description: ''
  name: common
  type: object
- description: Array of individual log records
  name: logs
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/log-api-log-data-object-schema.json
slug: log-api-log-data-object
source_filename: log-api-log-data-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/log-api-log-data-object-schema.json\",\n  \"title\": \"LogDataObject\",\n  \"description\": \"A batch of log records with optional shared attributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"common\": {\n      \"$ref\": \"#/components/schemas/CommonBlock\"\n    },\n    \"logs\": {\n      \"type\": \"array\",\n      \"description\": \"Array of individual log records\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LogRecord\"\n      },\n      \"example\": [\n        {\n          \"timestamp\": 1718153645993,\n          \"message\": \"Operation completed successfully\",\n          \"level\": \"FATAL\",\n          \"logtype\": \"standard\",\n          \"attributes\": {\n            \"customAttribute\": \"example_value\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"logs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/log-api-log-data-object-schema.json
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
title: LogDataObject
---
