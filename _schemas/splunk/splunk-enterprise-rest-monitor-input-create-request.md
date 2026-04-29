---
description: ''
layout: schema
name: MonitorInputCreateRequest
properties_list:
- description: The file or directory path to monitor
  name: name
  type: string
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
- description: Whether to create the input in disabled state
  name: disabled
  type: boolean
- description: Start monitoring from end of file
  name: followTail
  type: boolean
- description: Recursively monitor subdirectories
  name: recursive
  type: boolean
- description: Regex pattern for files to include
  name: whitelist
  type: string
- description: Regex pattern for files to exclude
  name: blacklist
  type: string
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-enterprise-rest-monitor-input-create-request-schema.json
slug: splunk-enterprise-rest-monitor-input-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MonitorInputCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The file or directory path to monitor\"\n    },\n    \"index\": {\n      \"type\": \"string\",\n      \"description\": \"Destination index\"\n    },\n    \"sourcetype\": {\n      \"type\": \"string\",\n      \"description\": \"Source type to assign\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source value to assign\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Host value to assign\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to create the input in disabled state\"\n    },\n    \"followTail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Start monitoring from end of file\"\n    },\n    \"recursive\": {\n      \"\
  type\": \"boolean\",\n      \"description\": \"Recursively monitor subdirectories\"\n    },\n    \"whitelist\": {\n      \"type\": \"string\",\n      \"description\": \"Regex pattern for files to include\"\n    },\n    \"blacklist\": {\n      \"type\": \"string\",\n      \"description\": \"Regex pattern for files to exclude\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-enterprise-rest-monitor-input-create-request-schema.json
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
title: MonitorInputCreateRequest
---
