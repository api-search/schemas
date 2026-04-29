---
description: ''
layout: schema
name: SearchJobCreateRequest
properties_list:
- description: The SPL search query to execute
  name: search
  type: string
- description: Earliest time for the search using relative or absolute time format
  name: earliest_time
  type: string
- description: Latest time for the search
  name: latest_time
  type: string
- description: The search mode
  name: search_mode
  type: string
- description: Execution mode. Normal runs asynchronously, oneshot runs synchronously, blocking waits for completion.
  name: exec_mode
  type: string
- description: Maximum number of results to return
  name: max_count
  type: integer
- description: Maximum time in seconds before the search is finalized
  name: max_time
  type: integer
- description: Number of seconds to keep the search after processing has stopped
  name: timeout
  type: integer
- description: Comma-separated list of required fields to include in results
  name: rf
  type: string
- description: Application namespace for the search
  name: namespace
  type: string
- description: Optional custom search ID. If not specified, Splunk generates one automatically.
  name: id
  type: string
- description: Number of status buckets to generate for the search timeline. Set to a value greater than 0 to enable timeline.
  name: status_buckets
  type: integer
- description: Seconds of inactivity after which the search is automatically cancelled. 0 means never auto-cancel.
  name: auto_cancel
  type: integer
- description: Auto-finalize the search after this number of events have been processed. 0 disables auto-finalize.
  name: auto_finalize_ec
  type: integer
- description: Seconds of inactivity after which the search is automatically paused. 0 means never auto-pause.
  name: auto_pause
  type: integer
- description: Whether to enable lookups during the search
  name: enable_lookups
  type: boolean
- description: Whether to reload macro definitions before the search
  name: reload_macros
  type: boolean
- description: How frequently to invoke the reduce phase (seconds)
  name: reduce_freq
  type: integer
- description: Whether to run the search in a separate process
  name: spawn_process
  type: boolean
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-enterprise-rest-search-job-create-request-schema.json
slug: splunk-enterprise-rest-search-job-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchJobCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"search\": {\n      \"type\": \"string\",\n      \"description\": \"The SPL search query to execute\"\n    },\n    \"earliest_time\": {\n      \"type\": \"string\",\n      \"description\": \"Earliest time for the search using relative or absolute time format\"\n    },\n    \"latest_time\": {\n      \"type\": \"string\",\n      \"description\": \"Latest time for the search\"\n    },\n    \"search_mode\": {\n      \"type\": \"string\",\n      \"description\": \"The search mode\"\n    },\n    \"exec_mode\": {\n      \"type\": \"string\",\n      \"description\": \"Execution mode. Normal runs asynchronously, oneshot runs synchronously, blocking waits for completion.\"\n    },\n    \"max_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of results to return\"\n    },\n    \"max_time\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"Maximum time in seconds before the search is finalized\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of seconds to keep the search after processing has stopped\"\n    },\n    \"rf\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of required fields to include in results\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Application namespace for the search\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Optional custom search ID. If not specified, Splunk generates one automatically.\"\n    },\n    \"status_buckets\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of status buckets to generate for the search timeline. Set to a value greater than 0 to enable timeline.\"\n    },\n    \"auto_cancel\": {\n      \"type\": \"integer\",\n      \"description\": \"Seconds of inactivity\
  \ after which the search is automatically cancelled. 0 means never auto-cancel.\"\n    },\n    \"auto_finalize_ec\": {\n      \"type\": \"integer\",\n      \"description\": \"Auto-finalize the search after this number of events have been processed. 0 disables auto-finalize.\"\n    },\n    \"auto_pause\": {\n      \"type\": \"integer\",\n      \"description\": \"Seconds of inactivity after which the search is automatically paused. 0 means never auto-pause.\"\n    },\n    \"enable_lookups\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable lookups during the search\"\n    },\n    \"reload_macros\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to reload macro definitions before the search\"\n    },\n    \"reduce_freq\": {\n      \"type\": \"integer\",\n      \"description\": \"How frequently to invoke the reduce phase (seconds)\"\n    },\n    \"spawn_process\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to run the search\
  \ in a separate process\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-enterprise-rest-search-job-create-request-schema.json
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
title: SearchJobCreateRequest
---
