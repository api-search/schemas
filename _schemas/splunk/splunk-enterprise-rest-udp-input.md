---
description: ''
layout: schema
name: UdpInput
properties_list:
- description: The UDP port number
  name: name
  type: string
- description: ''
  name: content
  type: object
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-enterprise-rest-udp-input-schema.json
slug: splunk-enterprise-rest-udp-input
source_filename: splunk-enterprise-rest-udp-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UdpInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The UDP port number\"\n    },\n    \"content\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-enterprise-rest-udp-input-schema.json
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
title: UdpInput
---
