---
description: LabelLinksBody schema
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
schema_file: json-schema/openapi-label-links-body-schema.json
slug: openapi-label-links-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-label-links-body-schema.json\",\n  \"title\": \"LabelLinksBody\",\n  \"description\": \"LabelLinksBody schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"servers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"example\": [\n        100\n      ]\n    },\n    \"applications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"example\": [\n        100\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-label-links-body-schema.json
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
