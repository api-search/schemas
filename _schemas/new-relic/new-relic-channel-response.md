---
description: ''
layout: schema
name: ChannelResponse
properties_list:
- description: ''
  name: channel
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-channel-response-schema.json
slug: new-relic-channel-response
source_filename: new-relic-channel-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"channel\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"configuration\": {\n          \"type\": \"object\",\n          \"example\": {},\n          \"properties\": {}\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"links\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"policy_ids\": {\n              \"type\": \"array\",\n              \"example\": [\n                100\n              ],\n              \"items\": {\n                \"type\": \"integer\"\n              }\n            }\n          }\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"example-resource-01\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"standard\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"ChannelResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-channel-response-schema.json
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
title: ChannelResponse
---
