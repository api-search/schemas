---
description: CreateUsagePlanRequest schema from Amazon API Gateway v1 API
layout: schema
name: CreateUsagePlanRequest
properties_list:
- description: Name of the usage plan.
  name: name
  type: string
- description: Description of the usage plan.
  name: description
  type: string
- description: ''
  name: throttle
  type: object
- description: ''
  name: quota
  type: object
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-create-usage-plan-request-schema.json
slug: v1-create-usage-plan-request
source_filename: v1-create-usage-plan-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the usage plan.\",\n      \"example\": \"my-resource\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the usage plan.\",\n      \"example\": \"A description of this resource.\"\n    },\n    \"throttle\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"burstLimit\": {\n          \"type\": \"integer\",\n          \"description\": \"Burst limit for requests.\",\n          \"example\": 49\n        },\n        \"rateLimit\": {\n          \"type\": \"number\",\n          \"description\": \"Steady-state rate limit (requests per second).\",\n          \"example\": 69.99\n        }\n      }\n    },\n    \"quota\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"limit\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of requests in the\
  \ period.\",\n          \"example\": 24\n        },\n        \"period\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"DAY\",\n            \"WEEK\",\n            \"MONTH\"\n          ],\n          \"description\": \"Time period (DAY, WEEK, MONTH).\",\n          \"example\": \"DAY\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-create-usage-plan-request-schema.json\",\n  \"title\": \"CreateUsagePlanRequest\",\n  \"description\": \"CreateUsagePlanRequest schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-create-usage-plan-request-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: CreateUsagePlanRequest
---
