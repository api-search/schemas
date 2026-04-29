---
description: ''
layout: schema
name: HecEvent
properties_list:
- description: Event timestamp in epoch time (seconds since 1970-01-01). If omitted, Splunk uses the current time.
  name: time
  type: string
- description: Hostname or IP address of the event source
  name: host
  type: string
- description: Source of the event
  name: source
  type: string
- description: Source type for the event
  name: sourcetype
  type: string
- description: Destination index for the event
  name: index
  type: string
- description: The event data. Can be a string or a JSON object. This is the actual data payload to be indexed.
  name: event
  type: string
- description: Additional metadata fields to associate with the event. These fields are indexed as metadata and can be searched.
  name: fields
  type: object
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-enterprise-rest-hec-event-schema.json
slug: splunk-enterprise-rest-hec-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HecEvent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"time\": {\n      \"type\": \"string\",\n      \"description\": \"Event timestamp in epoch time (seconds since 1970-01-01). If omitted, Splunk uses the current time.\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname or IP address of the event source\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source of the event\"\n    },\n    \"sourcetype\": {\n      \"type\": \"string\",\n      \"description\": \"Source type for the event\"\n    },\n    \"index\": {\n      \"type\": \"string\",\n      \"description\": \"Destination index for the event\"\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"The event data. Can be a string or a JSON object. This is the actual data payload to be indexed.\"\n    },\n    \"fields\": {\n     \
  \ \"type\": \"object\",\n      \"description\": \"Additional metadata fields to associate with the event. These fields are indexed as metadata and can be searched.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-enterprise-rest-hec-event-schema.json
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
title: HecEvent
---
