---
description: ''
layout: schema
name: IndexCreateRequest
properties_list:
- description: The name for the new index
  name: name
  type: string
- description: Type of data the index will hold
  name: datatype
  type: string
- description: Absolute path for hot and warm bucket storage
  name: homePath
  type: string
- description: Absolute path for cold bucket storage
  name: coldPath
  type: string
- description: Absolute path for thawed bucket storage
  name: thawedPath
  type: string
- description: Maximum total size of the index in MB
  name: maxTotalDataSizeMB
  type: integer
- description: Maximum size of a hot bucket
  name: maxDataSize
  type: string
- description: Seconds until data is frozen
  name: frozenTimePeriodInSecs
  type: integer
- description: Maximum number of hot buckets
  name: maxHotBuckets
  type: integer
- description: Maximum number of warm buckets
  name: maxWarmDBCount
  type: integer
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-enterprise-rest-index-create-request-schema.json
slug: splunk-enterprise-rest-index-create-request
source_filename: splunk-enterprise-rest-index-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IndexCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the new index\"\n    },\n    \"datatype\": {\n      \"type\": \"string\",\n      \"description\": \"Type of data the index will hold\"\n    },\n    \"homePath\": {\n      \"type\": \"string\",\n      \"description\": \"Absolute path for hot and warm bucket storage\"\n    },\n    \"coldPath\": {\n      \"type\": \"string\",\n      \"description\": \"Absolute path for cold bucket storage\"\n    },\n    \"thawedPath\": {\n      \"type\": \"string\",\n      \"description\": \"Absolute path for thawed bucket storage\"\n    },\n    \"maxTotalDataSizeMB\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum total size of the index in MB\"\n    },\n    \"maxDataSize\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum size\
  \ of a hot bucket\"\n    },\n    \"frozenTimePeriodInSecs\": {\n      \"type\": \"integer\",\n      \"description\": \"Seconds until data is frozen\"\n    },\n    \"maxHotBuckets\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of hot buckets\"\n    },\n    \"maxWarmDBCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of warm buckets\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-enterprise-rest-index-create-request-schema.json
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
title: IndexCreateRequest
---
