---
description: Channel schema
layout: schema
name: Channel
properties_list:
- description: ''
  name: channel
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-channel-schema.json
slug: openapi-channel
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-channel-schema.json\",\n  \"title\": \"Channel\",\n  \"description\": \"Channel schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channel\": {\n      \"$ref\": \"#/components/schemas/ChannelBody\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-channel-schema.json
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
title: Channel
---
