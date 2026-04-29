---
description: CloudWatchLogs schema from Amazon MSK API
layout: schema
name: CloudWatchLogs
properties_list:
- description: ''
  name: Enabled
  type: object
- description: ''
  name: LogGroup
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-cloud-watch-logs-schema.json
slug: msk-api-cloud-watch-logs
source_filename: msk-api-cloud-watch-logs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cloud-watch-logs-schema.json\",\n  \"title\": \"CloudWatchLogs\",\n  \"description\": \"CloudWatchLogs schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enabled\"\n          }\n        }\n      ]\n    },\n    \"LogGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"logGroup\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cloud-watch-logs-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CloudWatchLogs
---
