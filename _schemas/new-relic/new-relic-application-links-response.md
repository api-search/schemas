---
description: ''
layout: schema
name: ApplicationLinksResponse
properties_list:
- description: ''
  name: servers
  type: array
- description: ''
  name: application_hosts
  type: array
- description: ''
  name: application_instances
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-application-links-response-schema.json
slug: new-relic-application-links-response
source_filename: new-relic-application-links-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"servers\": {\n      \"type\": \"array\",\n      \"example\": [\n        100\n      ],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"application_hosts\": {\n      \"type\": \"array\",\n      \"example\": [\n        100\n      ],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"application_instances\": {\n      \"type\": \"array\",\n      \"example\": [\n        100\n      ],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationLinksResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-application-links-response-schema.json
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
title: ApplicationLinksResponse
---
