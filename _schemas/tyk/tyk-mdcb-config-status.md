---
description: ''
layout: schema
name: ConfigStatus
properties_list:
- description: ''
  name: listen_port
  type: integer
- description: ''
  name: healthcheck_port
  type: integer
- description: ''
  name: http_port
  type: integer
- description: ''
  name: enable_http_profiler
  type: boolean
- description: ''
  name: server_options
  type: object
- description: ''
  name: http_server_options
  type: object
- description: ''
  name: security
  type: object
- description: ''
  name: storage
  type: object
- description: ''
  name: analytics
  type: object
- description: ''
  name: hash_keys
  type: boolean
- description: ''
  name: session_timeout
  type: integer
- description: ''
  name: forward_analytics_to_pump
  type: boolean
- description: ''
  name: enable_multiple_analytics_keys
  type: boolean
- description: ''
  name: dont_store_selective
  type: boolean
- description: ''
  name: dont_store_aggregate
  type: boolean
- description: ''
  name: org_session_expiration
  type: integer
- description: ''
  name: org_session_cleanup
  type: integer
- description: ''
  name: license
  type: string
- description: ''
  name: aggregates_ignore_tags
  type: string
- description: ''
  name: track_all_paths
  type: boolean
- description: ''
  name: store_analytics_per_minute
  type: boolean
- description: ''
  name: ignore_tag_prefix_list
  type: string
- description: ''
  name: threshold_len_tag_list
  type: integer
- description: ''
  name: omit_analytics_index_creation
  type: boolean
- description: ''
  name: enable_separate_analytics_store
  type: boolean
- description: ''
  name: analytics_storage
  type: object
- description: ''
  name: log_level
  type: string
- description: ''
  name: enable_key_logging
  type: boolean
- description: ''
  name: sync_worker_config
  type: object
- description: ''
  name: enable_ownership
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-mdcb-config-status-schema.json
slug: tyk-mdcb-config-status
source_filename: tyk-mdcb-config-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConfigStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"listen_port\": {\n      \"type\": \"integer\"\n    },\n    \"healthcheck_port\": {\n      \"type\": \"integer\"\n    },\n    \"http_port\": {\n      \"type\": \"integer\"\n    },\n    \"enable_http_profiler\": {\n      \"type\": \"boolean\"\n    },\n    \"server_options\": {\n      \"type\": \"object\"\n    },\n    \"http_server_options\": {\n      \"type\": \"object\"\n    },\n    \"security\": {\n      \"type\": \"object\"\n    },\n    \"storage\": {\n      \"type\": \"object\"\n    },\n    \"analytics\": {\n      \"type\": \"object\"\n    },\n    \"hash_keys\": {\n      \"type\": \"boolean\"\n    },\n    \"session_timeout\": {\n      \"type\": \"integer\"\n    },\n    \"forward_analytics_to_pump\": {\n      \"type\": \"boolean\"\n    },\n    \"enable_multiple_analytics_keys\": {\n      \"type\": \"boolean\"\n    },\n   \
  \ \"dont_store_selective\": {\n      \"type\": \"boolean\"\n    },\n    \"dont_store_aggregate\": {\n      \"type\": \"boolean\"\n    },\n    \"org_session_expiration\": {\n      \"type\": \"integer\"\n    },\n    \"org_session_cleanup\": {\n      \"type\": \"integer\"\n    },\n    \"license\": {\n      \"type\": \"string\"\n    },\n    \"aggregates_ignore_tags\": {\n      \"type\": \"string\"\n    },\n    \"track_all_paths\": {\n      \"type\": \"boolean\"\n    },\n    \"store_analytics_per_minute\": {\n      \"type\": \"boolean\"\n    },\n    \"ignore_tag_prefix_list\": {\n      \"type\": \"string\"\n    },\n    \"threshold_len_tag_list\": {\n      \"type\": \"integer\"\n    },\n    \"omit_analytics_index_creation\": {\n      \"type\": \"boolean\"\n    },\n    \"enable_separate_analytics_store\": {\n      \"type\": \"boolean\"\n    },\n    \"analytics_storage\": {\n      \"type\": \"object\"\n    },\n    \"log_level\": {\n      \"type\": \"string\"\n    },\n    \"enable_key_logging\"\
  : {\n      \"type\": \"boolean\"\n    },\n    \"sync_worker_config\": {\n      \"type\": \"object\"\n    },\n    \"enable_ownership\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-mdcb-config-status-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: ConfigStatus
---
