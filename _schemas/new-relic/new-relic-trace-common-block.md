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
schema_file: json-schema/new-relic-trace-common-block-schema.json
slug: new-relic-trace-common-block
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Shared attributes applied to all spans in this batch\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value attributes applied to every span in the batch\",\n      \"example\": {\n        \"customAttribute\": \"example_value\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommonBlock\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-trace-common-block-schema.json
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
