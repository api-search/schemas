---
description: Shared attributes applied to all spans in this batch
layout: schema
name: CommonBlock
properties_list:
- description: Key-value attributes applied to every span in the batch
  name: attributes
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/trace-api-common-block-schema.json
slug: trace-api-common-block
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/trace-api-common-block-schema.json\",\n  \"title\": \"CommonBlock\",\n  \"description\": \"Shared attributes applied to all spans in this batch\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value attributes applied to every span in the batch\",\n      \"additionalProperties\": {\n        \"oneOf\": [\n          {\n            \"type\": \"string\"\n          },\n          {\n            \"type\": \"number\"\n          },\n          {\n            \"type\": \"boolean\"\n          }\n        ]\n      },\n      \"example\": {\n        \"customAttribute\": \"example_value\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/trace-api-common-block-schema.json
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
