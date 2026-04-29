---
description: ''
layout: schema
name: MonitorInputUpdateRequest
properties_list:
- description: Destination index
  name: index
  type: string
- description: Source type to assign
  name: sourcetype
  type: string
- description: Source value to assign
  name: source
  type: string
- description: Host value to assign
  name: host
  type: string
- description: Whether to disable the input
  name: disabled
  type: boolean
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-enterprise-rest-monitor-input-update-request-schema.json
slug: splunk-enterprise-rest-monitor-input-update-request
source_filename: splunk-enterprise-rest-monitor-input-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MonitorInputUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"index\": {\n      \"type\": \"string\",\n      \"description\": \"Destination index\"\n    },\n    \"sourcetype\": {\n      \"type\": \"string\",\n      \"description\": \"Source type to assign\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source value to assign\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Host value to assign\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to disable the input\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-enterprise-rest-monitor-input-update-request-schema.json
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
title: MonitorInputUpdateRequest
---
