---
description: ''
layout: schema
name: Paging
properties_list:
- description: Total number of items available
  name: total
  type: integer
- description: Number of items per page
  name: perPage
  type: integer
- description: Current offset
  name: offset
  type: integer
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-enterprise-rest-paging-schema.json
slug: splunk-enterprise-rest-paging
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Paging\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of items available\"\n    },\n    \"perPage\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items per page\"\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Current offset\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-enterprise-rest-paging-schema.json
tags:
- Analytics
- Data Analysis
- Logging
- Machine Data
- Monitoring
- Observability
- Platform
- Security
- SIEM
title: Paging
---
