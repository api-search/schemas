---
description: GetCurrentMetricDataResponse schema from Amazon Connect Service API
layout: schema
name: GetCurrentMetricDataResponse
properties_list:
- description: ''
  name: NextToken
  type: string
- description: ''
  name: MetricResults
  type: array
- description: ''
  name: DataSnapshotTime
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/get-current-metric-data-response-schema.json
slug: get-current-metric-data-response
source_filename: get-current-metric-data-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/get-current-metric-data-response-schema.json\",\n  \"title\": \"GetCurrentMetricDataResponse\",\n  \"description\": \"GetCurrentMetricDataResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"type\": \"string\"\n    },\n    \"MetricResults\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Dimensions\": {\n            \"type\": \"object\"\n          },\n          \"Collections\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Metric\": {\n                  \"type\": \"object\"\n                },\n                \"Value\": {\n                  \"type\": \"\
  number\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"DataSnapshotTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/get-current-metric-data-response-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: GetCurrentMetricDataResponse
---
