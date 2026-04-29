---
description: ''
layout: schema
name: IndexUpdateRequest
properties_list:
- description: Maximum total size of the index in MB
  name: maxTotalDataSizeMB
  type: integer
- description: Seconds until data is frozen
  name: frozenTimePeriodInSecs
  type: integer
- description: Maximum number of hot buckets
  name: maxHotBuckets
  type: integer
- description: Maximum number of warm buckets
  name: maxWarmDBCount
  type: integer
- description: Whether to disable the index
  name: disabled
  type: boolean
- description: Path to archive frozen buckets to. If not set, frozen data is deleted.
  name: coldToFrozenDir
  type: string
- description: Script to run when freezing buckets
  name: coldToFrozenScript
  type: string
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-enterprise-rest-index-update-request-schema.json
slug: splunk-enterprise-rest-index-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IndexUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxTotalDataSizeMB\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum total size of the index in MB\"\n    },\n    \"frozenTimePeriodInSecs\": {\n      \"type\": \"integer\",\n      \"description\": \"Seconds until data is frozen\"\n    },\n    \"maxHotBuckets\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of hot buckets\"\n    },\n    \"maxWarmDBCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of warm buckets\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to disable the index\"\n    },\n    \"coldToFrozenDir\": {\n      \"type\": \"string\",\n      \"description\": \"Path to archive frozen buckets to. If not set, frozen data is deleted.\"\n    },\n    \"coldToFrozenScript\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Script to run when freezing buckets\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-enterprise-rest-index-update-request-schema.json
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
title: IndexUpdateRequest
---
