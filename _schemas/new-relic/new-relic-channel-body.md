---
description: ''
layout: schema
name: ChannelBody
properties_list:
- description: ''
  name: configuration
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-channel-body-schema.json
slug: new-relic-channel-body
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"type\": \"object\",\n      \"example\": {},\n      \"properties\": {}\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChannelBody\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-channel-body-schema.json
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
title: ChannelBody
---
