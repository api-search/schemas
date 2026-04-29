---
description: ''
layout: schema
name: LabelBody
properties_list:
- description: ''
  name: category
  type: string
- description: ''
  name: links
  type: object
- description: ''
  name: name
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-label-body-schema.json
slug: new-relic-label-body
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"servers\": {\n          \"type\": \"array\",\n          \"example\": [\n            100\n          ],\n          \"items\": {\n            \"type\": \"integer\"\n          }\n        },\n        \"applications\": {\n          \"type\": \"array\",\n          \"example\": [\n            100\n          ],\n          \"items\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LabelBody\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-label-body-schema.json
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
title: LabelBody
---
