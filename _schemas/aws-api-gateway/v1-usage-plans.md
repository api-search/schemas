---
description: UsagePlans schema from Amazon API Gateway v1 API
layout: schema
name: UsagePlans
properties_list:
- description: ''
  name: items
  type: array
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-usage-plans-schema.json
slug: v1-usage-plans
source_filename: v1-usage-plans-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Usage plan identifier.\",\n            \"example\": \"abc123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Usage plan name.\",\n            \"example\": \"my-resource\"\n          },\n          \"throttle\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"burstLimit\": {\n                \"type\": \"integer\",\n                \"description\": \"Burst limit for requests.\",\n                \"example\": 49\n              },\n              \"rateLimit\": {\n                \"type\": \"number\",\n                \"description\": \"Steady-state rate limit (requests per second).\",\n                \"example\": 69.99\n        \
  \      }\n            }\n          },\n          \"quota\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"limit\": {\n                \"type\": \"integer\",\n                \"description\": \"Maximum number of requests in the period.\",\n                \"example\": 24\n              },\n              \"period\": {\n                \"type\": \"string\",\n                \"description\": \"Time period (DAY, WEEK, MONTH).\",\n                \"enum\": [\n                  \"DAY\",\n                  \"WEEK\",\n                  \"MONTH\"\n                ],\n                \"example\": \"DAY\"\n              }\n            }\n          }\n        }\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-usage-plans-schema.json\",\n  \"title\": \"UsagePlans\"\
  ,\n  \"description\": \"UsagePlans schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-usage-plans-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: UsagePlans
---
