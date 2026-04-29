---
description: ''
layout: schema
name: SearchJob
properties_list:
- description: The unique search ID
  name: sid
  type: string
- description: ''
  name: content
  type: object
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-enterprise-rest-search-job-schema.json
slug: splunk-enterprise-rest-search-job
source_filename: splunk-enterprise-rest-search-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchJob\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sid\": {\n      \"type\": \"string\",\n      \"description\": \"The unique search ID\"\n    },\n    \"content\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-enterprise-rest-search-job-schema.json
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
title: SearchJob
---
