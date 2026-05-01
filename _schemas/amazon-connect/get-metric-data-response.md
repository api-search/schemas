---
description: GetMetricDataResponse schema from Amazon Connect Service API
layout: schema
name: GetMetricDataResponse
properties_list:
- description: ''
  name: NextToken
  type: string
- description: ''
  name: MetricResults
  type: array
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/get-metric-data-response-schema.json
slug: get-metric-data-response
source_filename: get-metric-data-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/get-metric-data-response-schema.json\",\n  \"title\": \"GetMetricDataResponse\",\n  \"description\": \"GetMetricDataResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"type\": \"string\"\n    },\n    \"MetricResults\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Dimensions\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Queue\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"Id\": {\n                    \"type\": \"string\"\n                  },\n                  \"Arn\": {\n                    \"type\": \"string\"\n                  }\n                }\n       \
  \       },\n              \"Channel\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"Collections\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Metric\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"Name\": {\n                      \"type\": \"string\"\n                    },\n                    \"Unit\": {\n                      \"type\": \"string\"\n                    },\n                    \"Statistic\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                },\n                \"Value\": {\n                  \"type\": \"number\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/get-metric-data-response-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: GetMetricDataResponse
---
