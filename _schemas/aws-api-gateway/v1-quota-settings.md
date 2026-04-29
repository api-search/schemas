---
description: QuotaSettings schema from Amazon API Gateway v1 API
layout: schema
name: QuotaSettings
properties_list:
- description: Maximum number of requests in the period.
  name: limit
  type: integer
- description: Time period (DAY, WEEK, MONTH).
  name: period
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-quota-settings-schema.json
slug: v1-quota-settings
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of requests in the period.\",\n      \"example\": 24\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DAY\",\n        \"WEEK\",\n        \"MONTH\"\n      ],\n      \"description\": \"Time period (DAY, WEEK, MONTH).\",\n      \"example\": \"DAY\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-quota-settings-schema.json\",\n  \"title\": \"QuotaSettings\",\n  \"description\": \"QuotaSettings schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-quota-settings-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: QuotaSettings
---
