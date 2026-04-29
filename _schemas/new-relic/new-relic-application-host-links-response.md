---
description: ''
layout: schema
name: ApplicationHostLinksResponse
properties_list:
- description: ''
  name: application
  type: integer
- description: ''
  name: application_instances
  type: array
- description: ''
  name: server
  type: integer
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-application-host-links-response-schema.json
slug: new-relic-application-host-links-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"application_instances\": {\n      \"type\": \"array\",\n      \"example\": [\n        100\n      ],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"server\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationHostLinksResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-application-host-links-response-schema.json
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
title: ApplicationHostLinksResponse
---
