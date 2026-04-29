---
description: ChannelResponseType schema
layout: schema
name: ChannelResponseType
properties_list:
- description: ''
  name: configuration
  type: object
- description: ''
  name: id
  type: integer
- description: ''
  name: links
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-channel-response-type-schema.json
slug: openapi-channel-response-type
source_filename: openapi-channel-response-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-channel-response-type-schema.json\",\n  \"title\": \"ChannelResponseType\",\n  \"description\": \"ChannelResponseType schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"type\": \"object\",\n      \"properties\": {},\n      \"example\": {}\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"links\": {\n      \"$ref\": \"#/components/schemas/ChannelLinksResponse\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-channel-response-type-schema.json
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
title: ChannelResponseType
---
