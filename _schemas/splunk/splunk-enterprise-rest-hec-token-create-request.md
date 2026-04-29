---
description: ''
layout: schema
name: HecTokenCreateRequest
properties_list:
- description: Name for the new HEC token
  name: name
  type: string
- description: Default destination index
  name: index
  type: string
- description: Comma-separated list of allowed indexes
  name: indexes
  type: string
- description: Default sourcetype
  name: sourcetype
  type: string
- description: Default source value
  name: source
  type: string
- description: Default host value
  name: host
  type: string
- description: Whether to create the token in disabled state
  name: disabled
  type: boolean
- description: Whether to enable indexer acknowledgment
  name: useACK
  type: boolean
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-enterprise-rest-hec-token-create-request-schema.json
slug: splunk-enterprise-rest-hec-token-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HecTokenCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the new HEC token\"\n    },\n    \"index\": {\n      \"type\": \"string\",\n      \"description\": \"Default destination index\"\n    },\n    \"indexes\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of allowed indexes\"\n    },\n    \"sourcetype\": {\n      \"type\": \"string\",\n      \"description\": \"Default sourcetype\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Default source value\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Default host value\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to create the token in disabled state\"\n    },\n    \"useACK\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Whether to enable indexer acknowledgment\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-enterprise-rest-hec-token-create-request-schema.json
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
title: HecTokenCreateRequest
---
