---
description: ''
layout: schema
name: LabelLinksBody
properties_list:
- description: ''
  name: servers
  type: array
- description: ''
  name: applications
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-label-links-body-schema.json
slug: new-relic-label-links-body
source_filename: new-relic-label-links-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"servers\": {\n      \"type\": \"array\",\n      \"example\": [\n        100\n      ],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"applications\": {\n      \"type\": \"array\",\n      \"example\": [\n        100\n      ],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LabelLinksBody\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-label-links-body-schema.json
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
title: LabelLinksBody
---
